# KeyU 서버 v1.0.0

KeyU 서버 첫 공개 릴리스입니다. 스마트폰(KeyU 앱)을 PC의 텐키·트랙패드·매크로
패드로 사용할 수 있습니다. 모든 통신은 로컬 네트워크 안에서 암호화됩니다.

First public release of KeyU Server — use your phone (with the KeyU app) as a
numpad, trackpad, and macro pad for your PC. All traffic is encrypted and stays
on your local network.

## 구성물 / Assets

| 파일 | 대상 | SHA-256 |
|---|---|---|
| `KeyU 서버_1.0.0_aarch64.dmg` | macOS (Apple Silicon) | `745612ace097caf7824df00823be4fa2fe4b35606ec13397f17e4c4f4529f764` |
| `KeyU 서버_1.0.0_x64-setup.exe` | Windows 10+ x64 | `9b52ba220cf1ee5e7cd99f86fa43dadcede23acd87fa13581847685ec68cee9a` |

## 설치 요약 / Install notes

- 배포본은 아직 코드서명이 없습니다. macOS는 **우클릭 → 열기**로 1회 허용,
  Windows는 SmartScreen에서 **추가 정보 → 실행**을 선택하세요.
  Builds are unsigned for now — allow once via right-click → Open (macOS) or
  SmartScreen "More info → Run anyway" (Windows).
- macOS 입력 주입에는 손쉬운 사용(Accessibility) 권한이 필요합니다.
- 자세한 설치·연결 방법은 README를 참조하세요.

## 주요 기능 / Highlights

- 텐키 · 트랙패드 · 버튼 그리드 입력 모드, 매크로·버튼 편집, 시뮬레이션 바
- PIN/QR 최초 페어링 후 자동 재연결, 다중 서버 전환
- macOS ↔ Windows 서버 자동 인식(⌘/Ctrl 매핑), 한국어·영어
