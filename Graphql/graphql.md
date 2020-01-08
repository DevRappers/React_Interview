## Graphql에 대해서 설명해보시오.

> rest api와 비교하며 장점을 부각해서 설명하기.

graphql은 REST보다 효율적이고 강력하여 유연한 대안을 제공하는 새로운 API표준으로 알고 있습니다.
RestAPI와의 차이점을 들면서 설명을 해드리면
1. RestAPI는 여러개의 Endpoint를 가지는 반면 graphql은 한개의 Endpoint를 가집니다.
2. RestAPI는 Endpoint에 따라 데이터베이스 쿼리가 달라지는 반면 graphql은 스키마의 타입에 따라 쿼리가 달라집니다.
3. RestAPI의 over fetching문제점을 해결합니다. over fetching이란 예를 들어 학생의 정보에서 이름과 나이가 필요할 경우 Rest는 모든 정보를 불러와 필요없는 정보까지 불러오는 특성이 있는데 graphql은 원하는 것만 가져올 수 있기 때문에 이러한 문제가 해결됩니다.
4. RestAPI의 under fetching문제점을 해결합니다. under fetching이란 만약 사용자의 정보, feed정보를 가지고 오고 싶을 때 여러개의 API를 호출해야하는 그러한 특성이라고 알고 있는데 이 문제 역시 graphql은 원하는 정보만 쿼리로 가져올 수 있기 때문에 해결됩니다.

## Graphql의 동작방식/구조

Query와 Mutation이 schema에 구조를 정의하고 resolver에서 행동을 정의해서 schema에서 정의된 구조에 맞춰 클라이언트에서 Query, Mutation문으로 request를 하면 서버에서 JSON으로 반환하는 방식입니다.
   