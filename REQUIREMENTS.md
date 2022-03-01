# 요구사항 정리
## STEP 1 요구사항 - 최소 시간 경로 타입 추가
* [ ] 경로 조회 시 최소 시간 기준으로 조회할 수 있도록 기능을 추가하세요.
* [ ] 노선추가 & 구간 추가 시 거리와 함께 소요시간 정보도 추가하세요.
* [ ] 인수 테스트 (수정) -> 문서화 -> 기능 구현 순으로 진행하세요.
* [ ] 개발 흐름을 파악할 수 있도록 커밋을 작은 단위로 나누어 구현해보세요.
  
### 소요 시간 추가
* 경로 조회 시 총 소요 시간을 조회하기 위해서는 노선과 구간을 생성할 때 소요 시간 정보를 함께 보내야 합니다.
```
public class LineRequest {
  private String name;
  private String color;
  private Long upStationId;
  private Long downStationId;
  private int distance;
  private int duration;

  ...
```