# PROSPI 초기 코스트 도구

Windows 10/11 64비트용 실행 파일입니다. Python이나 Cheat Engine 설치는 필요하지 않습니다.

- [실행 파일 다운로드](https://github.com/dyoon125/code/raw/refs/heads/main/prospi-initial-cost/ProspiInitialCost.exe)
- [실행 파일 + 사용법 ZIP 다운로드](https://github.com/dyoon125/code/raw/refs/heads/main/prospi-initial-cost/ProspiInitialCost-v0.1-win64.zip)

## 기능

- 스타플레이어 어필 코스트 차감 방지
- 신규 선수 초기 능력치 코스트 차감 방지
- 해제하거나 정상 종료하면 이번 실행에서 읽은 원래 명령으로 복원

오리지널 선수 전용 코스트 유지 기능은 포함하지 않습니다. 이미 소모한 코스트를 채우는 기능도 아닙니다.

## 사용

1. 다른 에디터의 동일 기능을 끕니다.
2. 게임에서 해당 스타플레이어 생성 화면을 엽니다.
3. 프로그램에서 **게임 연결 / 다시 검색**을 누릅니다.
4. **명령 확인됨**으로 표시된 필요한 기능을 켭니다.
5. 생성 화면을 떠나기 전에 **둘 다 끄기 / 원래 코드 복원**을 누릅니다.

연결 대상은 `prospi-Win64-Shipping.exe`입니다. 생성 화면 자동 판별은 포함하지 않습니다. 명령 검색 결과가 없거나 모호하거나 다른 툴이 이미 변경한 경우에는 적용을 막습니다.

## 검증 범위

Windows x64 GUI 빌드, PE 형식과 시스템 DLL 의존성, 패턴 검색·경계 분할·중복 후보·이미 변경된 명령 판별 테스트를 통과했습니다. **실제 Windows 실행과 게임 적용·복원은 아직 검증하지 못했습니다.**

정상 종료 때 복원을 시도하며, 복원 실패 시 게임을 종료한 뒤 도구를 닫도록 안내합니다. 강제 종료는 복원을 보장하지 않습니다.

배포 파일 해시는 `prospi-initial-cost/SHA256SUMS.txt`에서 확인할 수 있습니다.
