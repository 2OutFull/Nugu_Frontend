#2사만루



##MLB
###게임
지금 MLB 게임 하고 있는거 있어?
이번 시즌 언제 시작해
이번 시즌 언제 끝나?
팀정리 (teams.json)
팀_active (teams_active.json)
선수별 스탯 (player stat) (하민, 지수)
{류현진} 최근 승률 알려줘
{류현진} ERA 알려줘
{류현진} {삼진} 몇개 잡았어?

경기 일정(팀별, 선수별) (https://api.sportsdata.io/v3/mlb/scores/json/Games/{season})
{류현진} 선수 지난 경기 일정 알려줘
{류현진} 선수 앞으로 경기 일정 알려줘
{류현진} 선수 오늘 경기 일정 알려줘
{텍사스 레인저스} 팀 지난 경기 일정 알려줘
{텍사스 레인저스} 팀 앞으로 경기 일정 알려줘

선수 vs 선수 승률 (https://api.sportsdata.io/v3/mlb/stats/json/HitterVsPitcher/{hitterid}/{pitcherid})
{류현진}이랑 {추신수} 역대 {대결 전적} 알려줘
{최지만}이 {게릿 콜}한테 {안타 칠 확률}이 몇이야?

용어설명 (terminology) : 하민
(http://m.mlb.com/glossary)
{WHIP} 이 뭐야?
{BABIP}이 뭐야?
{ERA}랑 {ERA+}랑 다른게 뭐야?


팀간 전적 (팀 vs 팀 승률) (https://sportsdata.io/developers/api-documentation/mlb#/team-stats)
  i. 	{~팀} 의 승률 알려줘
 ii. 	{~팀} 전적 알려줘  
iii. 	{~팀} 승률
iiii. 	{~팀} 전적
v. 	{~팀}과 {~팀} 

경기장별 승률 (park factor) : 
{어느 구장}이 제일 {투수 친화적}이야?


롤
팀정리 
ㅇㅇㅇ
ㅇㅇㅇ
축구

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
  
  
  https://baseball-in-play.com/90

https://developers-doc.nugu.co.kr/nugu-play/create-plays-with-play-builder/use-backend-proxy/backend-proxy-api-reference
