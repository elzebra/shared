### 배달음식을 주문하는 사람(소비자)을 위한 배달 앱


![배달의민족](https://play-lh.googleusercontent.com/8uMTbCdy6B93EGM5p6tfOVWnkDpee5ZOVYfaBgsWciG77nxZEpjltRtaOTxsI52x8Q=w240-h480)
![요기요](https://play-lh.googleusercontent.com/Zkel_nNv9Hq8met65g2HkbCYMoR0tZR5TaWaV5ZMqsfdwY3naycvlUKkarBJOWNPjpo=w240-h480)
![쿠팡이츠](https://play-lh.googleusercontent.com/VVxIA_jSqBzwzRSE9SXItUNLhT62QYdFNvCWT5msNIV_NXGJHi_C3GnyLvL14-niVQ=w240-h480)


> 4일 데이터 분석 플랫폼 모바일인덱스 등에 따르면 배민은 배달시장 점유율 67%로 압도적인 1위다. 요기요(23%)와 쿠팡이츠(10%)가 뒤를 잇고 있다. 배민을 운영하는 우아한형제들은 지난해 매출 2조9471억원에 순이익 2758억원을 거뒀다.

* https://www.hankyung.com/international/article/2023060488191


### 음식을 배달하는 사람(라이더)를 위한 배달 앱 


![배민커넥트](https://play-lh.googleusercontent.com/E0wErnxPojbZoZwtrAjDbcbQtQgiX7o-6t2nVc7cb7fUMHoYzGctdo4Uq5--PoaJZg=w240-h480)
![요기요라이더](https://play-lh.googleusercontent.com/dHerdt044sRf7WcbE6CAxC34WLdIzLTlM3aJfWiQWCngq3GqAq1XsEKeNEAoSiSIaQ=w240-h480)
![쿠팡이츠배달파트너](https://play-lh.googleusercontent.com/CA26DqKNezBnf2n5jSqfD_B7GTCz2vJoWStbEkoBMerEvRCftzU3_3vVTaiI2zCoUOA=w240-h480)

### 배달 음식을 판매하는 사람(음식점주)을 위한 배달 앱

![배민사장님](https://play-lh.googleusercontent.com/Q7LRIIqvL6wuJjCC_09z-io2ldL3NM3W572rS8wmEU_3kKzfc3v2ipaI7Tn1exdUg8g=w240-h480)
![요기요사장님](https://play-lh.googleusercontent.com/RqAaB4pqCbyAvIrbDQqmoNMBFAlNA9wSIZQGF9sk4GAmVBsWPbxuf33UWt3LWEQitYo=w240-h480)
![쿠팡이츠스토어](https://play-lh.googleusercontent.com/UGbWaMsPAX0zMUAzTypGiqznN5OQF07yNJGKCfomfpPgk8fTV2g-pPnxfuwGqdln4g=w240-h480)


### 음식 배달 플랫폼

* 위의 세 주체를 연결해주는 주체
  * 배달 음식을 만들어서 파는 사람(음식점주)
  * 음식을 배달해 주는 사람(라이더)
  * 음식을 주문해서 배달시키는 사람(소비자)

* 사용자들로부터 제공받은 혹은 사용자들이 생산한 데이터를 다른 데이들과 결합하고 가공하여 만들어낸 데이터를 이용하여 서비스를 제공하는 주체
* 나머지 세 주체는 배달 플랫폼 서비스의 이용자라는 공통점

* 돈의 흐름으로 보면 복잡한 관계
* 서비스의 이용 자체에 요금을 부과하는 사업모델은 성공하기 어려움, 예를 들어 네이버 포털 서비스, 카카오톡 메시징 서비스
* 서비스의 이용 자체에 요금을 부과하기 보다는 많은 무료 이용자를 끌어들여 서비스를 활성화시키고 사용자들의 데이터를 확보한 다음, 수익은 다른 방식으로 창출하는 것이 일반적임  
* 서비스의 이용자들의 서비스 이용에 대한 직접적인 요금 부담에 대한 회피 경향성은 플랫폼의 과점화의 중요한 원인 중의 하나
* (과점)플랫폼 사업자와 서비스 이용자의 불평등: 데이터의 비대칭성, 플랫폼이 정하는 규칙(알고리즘)에 종속, 최적 선택의 한계


### 클라이언트-서버 모델

* 서버
  * 서비스 제공자
  * 공개된 고정된 도메인명(IP 주소)을 가지고 있다.
  * 서버가 먼저 클라이언트와의 연결을 시도할 수 없다.
  * 클라이언트의 연결(접속) 요청을 수락하고 클라이언트의 요청에 대한 응답을 통해 데이터를 제공한다.
  
* 클라이언트
  * 서비스 이용자(의 기기에 설치된 앱)
  * 고정된 도메인명(IP 주소)을 가지고 있지 않다.
  * 항상 클라이언트 쪽에서 먼저 연결을 시도해야 한다.
  * 서버로의 연결(접속)을 시도하여 요청을 통해 데이터를 제공받는다.

### HTTP RESTful API

* IP/TCP/(TLS)/HTTP
* HTTP: text 기반, stateless(한 번의 연결에 한 쌍의 요청과 응답), header, path, method, body
* path로 자원(데이터)를 명시
* method(POST, GET, PUT, DELETE)로 해당 자원(데이터)에 대한 CRUD(Create, Retrieve, Update, Delete) 연산 종류를 명시
* API(application programming interface): 특정 server가 client(application)와 무슨 데이터를 어떻게 주고 받을지에 대한 약속
* Open API
  
### 배민커넥트

* 인증 서버: bros-riders-auth.woowa.in(52.79.169.53, 52.79.105.55)
* 데이터 서버: bros-riders.woowa.in(3.37.102.104, 3.38.8.0)

#### 로그인

요청
```
https://bros-riders-auth.woowa.in/oauth/token POST
```

응답
```
access_token                    : c59e8a5a-385d-41ed-a040-fb9db80c6447
token_type                      : bearer
refresh_token                   : d3c1efd2-221b-4f2c-a975-b7f55b866b98
expires_in                      : 604799
scope                           : read write trust
```

#### 배달 내역

요청
```
https://bros-riders.woowa.in/v1/api/me/rider-fee?fromDate=2022-06-01&toDate=2022-06-30 GET
```

응답
```
feeList
    deliveryId
        sn                              : 3441YMLJ
        bd                              : 20220626
    createdDate                     : 2022-06-26 15:44:34
    allocateDate                    : 2022-06-26 15:45:28
    orderId                         : T19H00007CW8
    deliveryStatus
        status
            code                            : COMPLETED_DELIVERY
            desc                            : 전달완료
    payable                         : True
    pickupOccurred                  : True
    riderFeePayable
        payable                         : True
        reason
            code                            : COMPLETED_PICKUP
            desc                            : 픽업완료 수행
        description                     : None
    reason                          : None
    locationDistanceKm              : 1.648
    actualLocationDistanceKm        : 1.648
    riderFeeCalculatedDistanceKm    : 1.648
    payableDeliveryFee              : 3800
    shopId                          : 13623567
    shopName                        : 에그드랍 롯데몰수지점
    agencyName                      : 경기동남점
    agencyId                        : 43
days                            : 31
allocateCount                   : 1
completeCount                   : 1
payableCount                    : 1
payableAmount                   : 3800
totalDistanceKm                 : 1.648
```


![](https://github.com/elzebra/test-actions/blob/main/photo_6168083185137727356_y.jpg?raw=true)


### 데이터 수집 방식

* 라이더의 스마트폰(안드로이드)에 앱 설치한다.
* 배민커넥트 API를 이용하여 로그인하고 자신의 배달내역 데이터를 가져온다.
* (라이더의 동의하에) 배달내역 데이터를 데이터 수집 서버로 전송한다.
* 라이더는 자신이 만들어낸 배달 내역 데이터에 대해 어느 정도의 통제권을 행사할 수 있는가?
* 배민커넥트 API를 배민커넥트 앱만이 사용할 수 있도록 만드는 것이 정당한가?
