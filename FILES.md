# 파일 안내

무기 판매 문제는 **이슈 보고서 → 당시 확인표 → 판매 처리 코드** 순서로 읽으면 수정 내용과 확인 결과를 함께 볼 수 있습니다. 구매·확장 비용은 경제 사례와 밸런스 시트를 연결해 정리했습니다.

## 소개와 자료 안내

| 파일 | 내용 |
|---|---|
| [프로젝트 소개](README.md) | 담당 업무, 대표 QA 사례, 출시 정보 |
| [코드 안내](code/README.md) | 세 가지 코드 발췌의 역할과 출처 |
| [밸런스 시트 안내](balance/README.md) | Excel 파일에 담긴 12개 시트의 내용 |

## 사례와 확인 기록

| 파일 | 내용 | 함께 볼 자료 |
|---|---|---|
| [판매한 무기가 계속 공격하는 문제](cases/04-weapon-sale.md) | 발생 조건, 기대·실제 결과, 수정 과정 | [당시 확인표](evidence/weapon-sale-checks.md), [판매 처리 코드](code/weapon-sale.cs.txt) |
| [무기 판매 확인표](evidence/weapon-sale-checks.md) | 레벨 구분, 확정·취소, 구매·합성의 당시 확인 결과 | [대표 이슈 보고서](cases/04-weapon-sale.md) |
| [자석 획득 효과](cases/01-magnet.md) | 획득 범위의 차이를 느끼기 어려웠던 상황과 수정 후 플레이 결과 | [획득 반경 계산](code/magnet-range.cs.txt) |
| [한글 표시](cases/02-ui-text.md) | 업그레이드 제목·설명이 네모로 보이던 문제와 표시 확인 | 보조 UI 사례 |
| [구매와 가방 확장 비용](cases/03-economy.md) | 114골드에서 구매·확장을 함께 하기 어려웠던 상황과 조정안 | [밸런스 시트](balance/project2-balance-v5-ko.xlsx), [상점 진입 코드](code/shop-entry.cs.txt) |
| [진화 무기 조정](cases/05-evolved-weapons.md) | 공격 반경과 분열 단계 제한, 이펙트 표시 조정 | [조정 전 플레이 화면](evidence/evolved-weapons-before.jpg) |

## 코드와 밸런스 시트

| 파일 | 내용 |
|---|---|
| [무기 판매 처리](code/weapon-sale.cs.txt) | 판매 결과에 담긴 아이템 ID·레벨을 실제 무기 제거 이벤트로 전달 |
| [획득 반경 계산](code/magnet-range.cs.txt) | 기본 획득 반경에 로비 업그레이드 비율을 적용하는 계산 |
| [상점 진입 판단](code/shop-entry.cs.txt) | 누적 획득 목표와 진입비, 진입 후 남을 골드를 구분하는 계산 |
| [밸런스 조정안 v5](balance/project2-balance-v5-ko.xlsx) | 비용·성장·전투 수치와 플레이 측정 양식을 담은 Excel 파일 |

## 플레이 이미지

| 파일 | 내용 |
|---|---|
| [일반 전투 화면](evidence/inventory-playtest.jpg) | 게임 구성과 전투 화면을 소개하는 2026년 7월 플레이 장면 |
| [진화 무기 조정 전 화면](evidence/evolved-weapons-before.jpg) | 큰 오라와 여러 무기 궤적이 화면을 차지하던 장면 |

일반 전투 이미지는 게임 화면을 소개하기 위해 넣었습니다. 판매 버그의 수정 결과는 당시 확인표에서 볼 수 있습니다.
