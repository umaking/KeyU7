# KeyU 서버

**스마트폰을 PC의 텐키·트랙패드·매크로 패드로.**
KeyU 앱(iOS·Android)과 같은 Wi-Fi에 있는 PC에서 이 서버를 실행하면, 폰이 곧바로
PC의 입력 장치가 됩니다. 모든 통신은 로컬 네트워크 안에서 암호화되어 이루어지며,
외부 서버를 거치지 않습니다.

*(English guide below — [English](#keyu-server-english))*

## 다운로드

최신 버전은 **[Releases](releases)** 페이지에서 받을 수 있습니다.

| 플랫폼 | 파일 | 요구 사항 |
|---|---|---|
| macOS (Apple Silicon) | `KeyU 서버_<버전>_aarch64.dmg` | 손쉬운 사용(Accessibility) 권한 |
| Windows x64 | `KeyU 서버_<버전>_x64-setup.exe` | Windows 10 이상 64비트 |

무결성 확인: 각 릴리스에 첨부된 `SHA256SUMS`와 대조하세요.
`shasum -a 256 <파일>` (macOS) / `certutil -hashfile <파일> SHA256` (Windows)

## 설치

**macOS** — dmg를 열어 `KeyU 서버.app`을 응용 프로그램에 끌어 넣습니다.
현재 배포본은 개발자 서명·공증이 없어 최초 실행 시 Gatekeeper가 차단합니다 —
앱을 **우클릭 → 열기**(또는 시스템 설정 → 개인정보 보호 및 보안 → "그래도 열기")로
1회 허용하세요. 입력 주입에는 **손쉬운 사용(Accessibility) 권한**이 필요합니다
(첫 실행 시 안내가 표시됩니다).

**Windows** — `x64-setup.exe`를 실행합니다. 서명이 없어 SmartScreen 경고가 뜹니다 —
**"추가 정보 → 실행"**을 누르세요. 로컬 네트워크 수신을 위한 방화벽 예외를 허용하세요.

## 연결

1. PC에서 KeyU 서버 실행 (메뉴 막대/트레이에 상주)
2. 폰의 KeyU 앱이 같은 Wi-Fi에서 서버를 자동 발견
3. 서버 창의 6자리 PIN 입력 또는 QR 스캔으로 최초 페어링 — 이후에는 자동 재연결

## 주요 기능

- **텐키 · 트랙패드 · 버튼 그리드** 3가지 입력 모드
- **매크로**: 키 시퀀스·지연·텍스트 입력을 버튼 하나로
- **버튼·레이아웃 편집**: 프리셋 관리, 분할 버튼, 시뮬레이션 바
- **다중 서버**: 여러 PC를 페어링해 두고 탭 한 번으로 전환
- macOS ↔ Windows 서버 자동 인식(⌘/Ctrl 매핑 전환), 한국어·영어 지원

## 개인정보

서버는 계정·로그인 없이 동작하며 어떤 데이터도 수집·전송하지 않습니다.
키 입력은 로컬 네트워크 안에서 암호화 전송 후 즉시 주입되고 기록되지 않습니다.
앱을 포함한 전체 개인정보 처리방침: **<개인정보 처리방침 URL — 게시 후 교체>**

## 라이선스

KeyU 서버는 **무료 소프트웨어**입니다(재배포·수정 불가 — [LICENSE](LICENSE) 참조).
포함된 오픈소스 구성요소 목록은 [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md)에 있습니다.

---

# KeyU Server (English)

**Turn your phone into a numpad, trackpad, and macro pad for your PC.**
Run this server on a PC that shares Wi-Fi with the KeyU app (iOS/Android), and
your phone becomes an input device. All traffic stays encrypted on your local
network — no external servers involved.

## Download

Get the latest build from the **[Releases](releases)** page.

| Platform | File | Requirements |
|---|---|---|
| macOS (Apple Silicon) | `KeyU 서버_<version>_aarch64.dmg` | Accessibility permission |
| Windows x64 | `KeyU 서버_<version>_x64-setup.exe` | Windows 10+ (64-bit) |

Verify downloads against the `SHA256SUMS` file attached to each release.

## Install

**macOS** — Open the dmg and drag `KeyU 서버.app` into Applications. Builds are
currently unsigned/un-notarized, so Gatekeeper blocks the first launch —
**right-click → Open** (or System Settings → Privacy & Security → "Open Anyway")
once. Input injection requires the **Accessibility** permission (you'll be
prompted on first run).

**Windows** — Run `x64-setup.exe`. The build is unsigned, so SmartScreen will
warn — click **"More info → Run anyway"**. Allow the firewall exception for
local-network listening.

## Connect

1. Launch KeyU Server on your PC (it lives in the menu bar / tray)
2. The KeyU app discovers the server automatically on the same Wi-Fi
3. Pair once with the 6-digit PIN or QR shown by the server — reconnection is automatic afterwards

## Privacy

The server runs without accounts and collects or transmits no data. Keystrokes
are encrypted on your local network, injected immediately, and never logged.
Full privacy policy (including the mobile apps): **<privacy policy URL>**

## License

KeyU Server is **free software** (no redistribution/modification — see
[LICENSE](LICENSE)). Bundled open-source components are listed in
[THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).
