# 관련 코드 발췌

사례를 설명할 때 참고할 수 있도록 Unity C# 코드 세 부분을 가져왔습니다.

| 코드 | 연결되는 사례 | 내용 |
|---|---|---|
| [무기 판매 처리](weapon-sale.cs.txt) | [판매 후 공격 잔존](../cases/04-weapon-sale.md) | 판매한 아이템의 ID·레벨을 실제 무기 제거 이벤트에 전달 |
| [획득 반경 계산](magnet-range.cs.txt) | [자석 체감 개선](../cases/01-magnet.md)의 계산 참고 | 로비 업그레이드가 획득 반경에 반영되는 계산. 자석 패시브의 전체 수정 내용은 포함하지 않음 |
| [상점 진입 판단](shop-entry.cs.txt) | [구매·성장 흐름](../cases/03-economy.md) | 진행 목표·진입 비용·진입 후 잔여 골드 확인 |

판매 처리는 2026년 10월 1일 `InventoryUiService.cs`에서, 나머지 두 발췌는 9월 30일 `PlayerStatManager.cs`와 `PlayerLevelManager.cs`에서 가져왔습니다. 각 날짜에 가져온 구현의 일부로, 수정 전후를 비교한 자료는 아닙니다.
