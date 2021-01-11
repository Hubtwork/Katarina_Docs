## KATALINA [ League Of Legends Info Platform ]

---

> ver 0.1
>
> - Katalina_DataDragon Loader
> - Katalina_League API





### API

---

#### 

### Summoner - V1

------

<span style = 'background:red; color:white;'> GET </span>	/api/summoner/v1/summonerInfo/{summonerName}

##### Response Classes

##### Return Value : SummonerDataDTO

---

**SummonerDataDTO**

| Name         | Data Type             | Description           |
| ------------ | --------------------- | --------------------- |
| summonerInfo | SummonerInfoDTO       | 소환사 기본 정보      |
| records      | ArrayList [RecordDTO] | 소환사 랭크 티어 정보 |

##### SummonerInfoDTO

| Name          | Data Type | Description                                |
| ------------- | --------- | ------------------------------------------ |
| revision Date | Long      | 마지막 갱신 일자 ( Long - Date 치환 필요 ) |
| name          | String    | 현재 소환사명                              |
| summonerLevel | Long      | 현재 소환사 레벨                           |
| profileIconId | Int       | 현재 사용중인 프로필 아이콘 ID             |

##### RecordDTO

| Name        | Data Type | Description                                                  |
| ----------- | --------- | ------------------------------------------------------------ |
| type        | String    | 게임 타입 ( 칼바람, 솔로랭크, 자유랭크 등 ) ( v1 은 칼바람 미지원 ) |
| tier        | String    | 현재 티어 ( 티어 / 단계 / 포인트 병합 문자열 제공 )          |
| win         | Int       | 해당 게임 승리 수                                            |
| lose        | Int       | 해당 게임 패배 수                                            |
| winningRate | Double    | 승률 ( 소수점 두자리 까지 표현 )                             |

---



