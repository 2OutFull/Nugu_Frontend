# 2사만루



## MLB
### 게임
지금 MLB 게임 하고 있는거 있어?
이번 시즌 언제 시작해
이번 시즌 언제 끝나?
팀정리 (teams.json)
팀_active (teams_active.json)
선수별 스탯 (player stat) (하민, 지수)
{류현진} 최근 승률 알려줘
{류현진} ERA 알려줘
{류현진} {삼진} 몇개 잡았어?

### 경기 일정(팀별, 선수별) (https://api.sportsdata.io/v3/mlb/scores/json/Games/{season})
#### e-1. 팀
{텍사스 레인저스} 팀 지난 경기 일정 알려줘
{텍사스 레인저스} 팀 앞으로 경기 일정 알려줘

#### e-2. 선수
{류현진} 선수 지난 경기 일정 알려줘
{류현진} 선수 앞으로 경기 일정 알려줘
{류현진} 선수 오늘 경기 일정 알려줘

### 선수 vs 선수 승률 (https://api.sportsdata.io/v3/mlb/stats/json/HitterVsPitcher/{hitterid}/{pitcherid})
{류현진}이랑 {추신수} 역대 {대결 전적} 알려줘
{최지만}이 {게릿 콜}한테 {안타 칠 확률}이 몇이야?

### 용어설명 (terminology) : 하민
(http://m.mlb.com/glossary)
{WHIP} 이 뭐야?
{BABIP}이 뭐야?
{ERA}랑 {ERA+}랑 다른게 뭐야?


### 팀간 전적 (팀 vs 팀 승률) (https://sportsdata.io/developers/api-documentation/mlb#/team-stats) <br>
  i. 	{~팀} 의 승률 알려줘 <br>
 ii. 	{~팀} 전적 알려줘  <br>
iii. 	{~팀} 승률 <br>
iiii. 	{~팀} 전적 <br>
v. 	{~팀}과 {~팀} <br>

### 경기장별 승률 (park factor) : 
{어느 구장}이 제일 {투수 친화적}이야?


## 롤
팀정리 
ㅇㅇㅇ
ㅇㅇㅇ
## 축구

“””
<START>
mkdir test_mlb && cd test_mlb
python3 -m venv venv
./venv/bin/activate.bat

python  // 파이썬 interactive command
import statsapi
from pprint import pprint
pprint(statsapi.schedule(team=133,start_date='01/01/2019',end_date='12/31/2019'))
“””


>>> pprint(statsapi.lookup_player("ryu"))
[{'boxscoreName': 'Ryu',
  'currentTeam': {'id': 119},
  'firstLastName': 'Hyun-Jin Ryu',
  'firstName': 'Hyun-Jin',
  'fullFMLName': 'Hyun-Jin Ryu',
  'fullLFMName': 'Ryu, Hyun-Jin',
  'fullName': 'Hyun-Jin Ryu',
  'id': 547943,
  'initLastName': 'H Ryu',
  'lastFirstName': 'Ryu, Hyun-Jin',
  'lastInitName': 'Ryu, H',
  'lastName': 'Ryu',
  'mlbDebutDate': '2013-04-02',
  'nameFirstLast': 'Hyun-Jin Ryu',
  'nickName': 'Monster',
  'primaryNumber': '99',
  'primaryPosition': {'abbreviation': 'P', 'code': '1'},
  'useName': 'Hyun-Jin'}]

## ★여기서부터 예상발화★
서술어, 어미, entity 조합, 어순 및 문장구조

경기일정 (팀별, 선수별)
parameters : {player}, {team}
예상발화: {player} 선수 or {team} 팀 경기 일정 알려줘

{player} : [추신수, 류현진, 정호, 승환, 박지만(지만)]
{team} : 


지원&재희
팀





### 선수
야구 결과 / 야구 경기 / 야구 시합결과 / 시합 결과
결과 알려줘 / 알고 싶어 /  알려줄래 / 어떻게 됐어 / 이겼어? / 어떻게 끝났는지 말해줄래 / 어떻게 됐는지 확인 부탁해

{류현진} 선수 과거
야구
일정
알려줘
{류현진} 선수 지난 
야구 경기
스케줄
말해줘
{류현진} 선수 어제
야구 시합
계획
알고 싶어
{류현진} 선수 오늘
경기
날짜
알려줄래?
{류현진} 선수 최근
시합


어떻게 돼?
{류현진} 선수 내일
매치


어때?
{류현진} 선수 앞으로
야구 게임


말해줄래?
{류현진} 선수 미래
야구 플레이


언제야?


플레이


언제 해?






있어?






없어?






있는 지 알려줘






언제 할까?






언제인지 알아?


### 지수&영훈 (선수 스탯)
parameters : {player}, {stat}
예상발화: {player} {stat} 알려줘
{player} : [추신수, 류현진, 정호, 승환, 최지만(지만)]
{stat} : [게임수, 땅볼 아웃, 플라이(뜬공) 아웃, 






>>> {  추신수(타자, hitting) 강정호, 최지만
    "gamesPlayed": 1619,  	출장횟수
    "groundOuts": 1737,	땅볼아웃
    "airOuts": 1188,		플라이아웃
    "runs": 948,		득점
    "doubles": 336,		2루타, 이루타
    "triples": 29,		3루타, 삼루타
    "homeRuns": 213,		홈런
    "strikeOuts": 1546,	삼진아웃
    "baseOnBalls": 855,	볼넷
    "intentionalWalks": 42,		고의사구
    "hits": 1645,		안타
    "hitByPitch": 150,	데드볼
    "avg": ".275",		타율
    "atBats": 5977,		타수
    "obp": ".377",		출루율
    "slg": ".448",		장타율
    "ops": ".826",		OPS
    "caughtStealing": 53,    도루사, 도루자, 도루저지
    "stolenBases": 151,	도루
    "stolenBasePercentage": ".740",	도루성공률
    "groundIntoDoublePlay": 100,	더블플레이
    "numberOfPitches": 28474,		투구수 
    "plateAppearances": 7030,		타석수 
    "totalBases": 2678,		총 루타수		
    "rbi": 767,			득점타 
    "leftOnBase": 2155,		잔루
    "sacBunts": 10,			희생번
    "sacFlies": 38,			희생플라이
    "babip": ".336",			바빕, 
    "groundOutsToAirouts": "1.46", 	땅볼아웃/뜬공아웃 비율
    "atBatsPerHomeRun": "28.06"	홈런 타율
}


>>> { 투수 류현진, 오승환
   "gamesPlayed": 29,		경기수, 출장수
    "gamesStarted": 29,	선발 수
    "groundOuts": 231,	땅볼 아웃
    "airOuts": 141,		뜬공 아웃
    "runs": 53,		실점
    "homeRuns": 17,		피홈런
    "strikeOuts": 163,	삼진아웃
    "baseOnBalls": 24,	볼넷
    "intentionalWalks": 2,	고의사구
    "hits": 160,		피안타
    "avg": ".234",		피안타율
    "atBats": 685,		타석수
    "obp": ".263",		출루율
    "slg": ".359",		피 장타율
    "ops": ".622",		OPS
    "caughtStealing": 1,	도루사
    "stolenBases": 1,		도루
    "stolenBasePercentage": ".500",		도루성공확률
    "groundIntoDoublePlay": 17,		더블플레이
    "numberOfPitches": 2706,			투구 수
    "era": "2.32",				평균자책점
    "inningsPitched": "182.2",		투구 이닝
    "wins": 14,				승리수
    "losses": 5,				패배수
    "saves": 0,				세이브수
    "saveOpportunities": 0,			세이브 기회
    "holds": 0,				홀드
    "earnedRuns": 47,				실점
    "whip": "1.01",				WHIP
    "battersFaced": 723,			상대한 타자 수
    "gamesPitched": 29,			투구 경기 수
    "completeGames": 1,			완투
    "shutouts": 1,				완봉
    "strikes": 1799,				스트라이크
    "strikePercentage": "66.5",		스트라이크 비율
    "hitBatsmen": 4,				몸에 맞는 공
    "balks": 0,				보크
    "wildPitches": 0,				폭투
    "pickoffs": 2,				견제구
    "groundOutsToAirouts": "1.64",		땅볼 플라이볼 비율
    "winPercentage": ".737",			승률
    "pitchesPerInning": "14.8",		이닝 당 투구 수
    "gamesFinished": 0,		경기 종료 투수
    "strikeoutWalkRatio": "6.79",	삼진 볼넷 비율
    "strikeoutsPer9Inn": "8.03",	9이닝 당 스트라이크 수
    "walksPer9Inn": "1.18",		9이닝 당 볼넷 수, 9이닝 당 4구 수
    "hitsPer9Inn": "7.88",		9이닝 당 안타 수
    "runsScoredPer9": "5.57",		9이닝 당 득점 수
    "homeRunsPer9": "0.84",		9이닝 당 홈런 수
    "inheritedRunners": 0,		승계주자
    "inheritedRunnersScored": 0	승계주자 득점율
}

  
  
  https://baseball-in-play.com/90

https://developers-doc.nugu.co.kr/nugu-play/create-plays-with-play-builder/use-backend-proxy/backend-proxy-api-reference

https://sites.google.com/site/eveningglow17/record/yagu-yong-eo-jeongli
