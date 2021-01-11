



### STATICS

---

> Game Constants.

1. Seasons

- 시즌 정보 조회 :: Format [ id, season ]
  - Endpoint : http://static.developer.riotgames.com/docs/lol/seasons.json
  - Match 정보 등에서 id 값으로 제공되는 시즌 정보 매핑

2. Queue Ids

- 큐 정보 조회 :: Format [ queueId, map, description, notes ]
  - Endpoint : http://static.developer.riotgames.com/docs/lol/queues.json
  - LoL API 내에서 제공되는 QueueId 연관 정보 제공

3. Maps

- 맵 정보 조회 :: Format [ mapId, mapName, notes ]
  - Endpoint : http://static.developer.riotgames.com/docs/lol/maps.json
  - LoL 맵 정보 제공

4. Game Modes

- 게임 모드 조회 :: Fomat [ gameMode, description ]
  - Endpoint : http://static.developer.riotgames.com/docs/lol/gameModes.json
  - LoL 게임 모드 정보 제공 ( 협곡, 우르프, 오디세이 등 )

5. Game Types

- 게임 타입 조회 :: Format [ gameType, description ]
  - Endpoint : http://static.developer.riotgames.com/docs/lol/gameTypes.json
  - LoL 게임 타입 제공 ( 사용자 정의, 튜토리얼, 매치 )



### Data Dragon

---

>Centralized LoL game data, assets.



#### API

---

> Base URL : [https://ddragon.leagueoflegends.com/api/](https://ddragon.leagueoflegends.com/api/)

1. Versions

- 사용가능한 Data Dragon 버전 목록 조회 ( 최신 버전 유지 필요 )
  - Endpoint : **versions.json**
  - Full URL : [https://ddragon.leagueoflegends.com/api/versions.json](https://ddragon.leagueoflegends.com/api/versions.json)

sp

#### REALMS

---

> Base URL : [https://ddragon.leagueoflegends.com/realms/](https://ddragon.leagueoflegends.com/realms)

1. Realms

- 지역 ( Region ) 별 현재 Data Dragon 버전 조회
  - Endpoint : **{localeName}.json**
  - Full URL : [https://ddragon.leagueoflegends.com/realms/kr.json](https://ddragon.leagueoflegends.com/realms/kr.json)



#### CDN

---

> Base URL : https://ddragon.leagueoflegends.com/cdn/
>
> LoL game data, assets.
>
> 

1. Languages

- 롤 지원 언어 조회
  - Endpoint: **languages.json**
  - Full URL : https://ddragon.leagueoflegends.com/cdn/languages.json



#### CDN - DATA

---

>Base URL : http://ddragon.leagueoflegends.com/cdn/10.25.1/data/ko_KR/
>
>		- 10.25.1 :: variable_DataDragon Version
>		- ko_KR :: variable_Language Code
>
>Provide LoL game data.
>
>

1. Champion

- 전체 챔피언 정보 조회
  - Endpoint: **champion.json**
  - Full URL : http://ddragon.leagueoflegends.com/cdn/10.25.1/data/ko_KR/champion.json
- 특정 챔피언 정보 조회
  - Endpoint : **champion/{ 챔피언 Key ID }.json**
  - Full URL : http://ddragon.leagueoflegends.com/cdn/10.25.1/data/ko_KR/champion/{ 챔피언 Key ID }.json

2. 

