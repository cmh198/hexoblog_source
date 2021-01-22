---
title: Cache
categories: 
- CS
- 컴퓨터 구조
- Cache
tag: 
- 컴퓨터 구조
- Cache
- 캐시
---
## Cache란 무엇인가?
___
- Cache는 CPU와 메인 메모리 사이에 존재하고, CPU가 데이터에 접근할 때 마다 메인 메모리까지 가기에는 cost가 너무 크기 때문에 그 사이에 Cache를 두어 자주 사용하는 data를 저장해 놓고 CPU는 특정 데이터가 필요할 때 그 데이터가 Cache에 있는지 우선적으로 탐색한다. 만약 찾지 못했다면 miss 처리를 한 뒤 메모리에서 그 데이터를 Cache에 적재한다.

![메모리 Hierachy](https://user-images.githubusercontent.com/29699750/104117657-530c0b80-5366-11eb-97e6-5a83597ba1fb.PNG)

## Locality의 원리
- 캐시에 데이터를 적재할 때 어떤 기준을 두고 적재하게 된다. 그 기준이 바로 Locality이다. Locality는 두 가지 종류가 있는데 시간 지역성과 공간 지역성이 있다.
- Temporal Locality
    - 시간 지역성은 최근 접근한 데이터를 다시 접근할 확률이 높음을 뜻한다.
- Spatial Locality
    - 공간 지역성은 접근한 데이터의 주변(메모리 주소와 인접한)을 다시 접근할 확률이 높음을 뜻한다.
___



## Cache miss

1. Conpulsory miss(Cold miss)
- 캐시를 맨 처음 접근할 때 발생하는 miss 
    - 초기 상태의 캐시는 비어있기 때문에 miss가 반드시 발생한다.(피할 수 없다)
2. Capacity miss
- Capacity가 부족해서 발생하는 miss
    - 교체 정책을 통해 사용한지 오래된 데이터는 바꿔준다.
3. Conflict miss
- Direct-mapped Cache에서 발생하는 miss이다. 
    - 두 데이터를 저장할 때 같은 index를 가리킨다면 어떤 데이터를 저장할지 컴퓨터는 모르기 때문에 발생한다.
    -> way가 부족해서 나타나는 현상이므로 way를 늘려준다.

## Cache




