# Windows에서 ThreeMod 자동 설치하기

이 문서와 같은 GitHub Release의 `install-byc-windows.ps1`을 ChatGPT/Codex에 전달하고 **“ThreeMod를 설치하고 실행해줘. 생성은 하지 마”**라고 요청하세요. 로컬 명령 실행이 가능한 에이전트가 다운로드·검증·설치·앱 실행을 처리합니다. 일반 웹 채팅만으로는 PC 설치를 실행할 수 없습니다.

## 에이전트 실행 절차

1. [공식 최신 Release](https://github.com/Niceofer/ThreeMod/releases/latest)의 `install-byc-windows.ps1`을 파일로 다운로드합니다. 이 첨부 파일은 해당 변경이 포함된 다음 Release부터 제공됩니다. 다운로드한 코드를 즉시 문자열로 실행하지 말고 파일로 확인합니다.
2. 사용자가 설치를 요청한 뒤 다음 명령을 실행합니다. 경로는 로컬에서 받은 실제 파일 경로로 바꿉니다.

```powershell
# PowerShell 세션에서 실행 (Windows PowerShell 또는 PowerShell 7)
& .\install-byc-windows.ps1
```

스크립트는 설치형 `ThreeMod-Setup-버전.exe`만 선택하고 GitHub asset의 파일 크기 및 SHA-256을 확인합니다. portable 파일은 설치 대상으로 사용하지 않습니다. 해시 누락·불일치, 다운로드 오류에서는 설치를 중단합니다.

3. Windows SmartScreen이나 관리자 권한 승인이 표시되면 사용자에게 처리하도록 안내하고 기다립니다. 경고가 항상 표시되는 것은 아니며, 취소나 보안 정책 차단 시 자동 설치가 완료되지 않습니다. `Unblock-File`, Zone.Identifier 삭제, 보안 설정 변경을 하지 않습니다. PowerShell 실행 정책이 스크립트를 차단해도 우회하지 말고 관리자 정책 또는 수동 설치로 안내합니다.
4. 설치가 끝나면 ThreeMod를 실행합니다. 사용자가 로그인한 뒤 옵션에서 **로컬 연결 허용 → 플러그인 소스 등록**을 진행합니다. ChatGPT를 다시 시작하고 ThreeMod 플러그인을 설치·활성화합니다.
5. 프로젝트와 노드 조회만 확인합니다. 설치 검증 과정에서 생성 도구를 실행하지 않습니다.

## 기존 설치와 버전 선택

이미 설치된 ThreeMod가 있으면 기본적으로 다시 설치하지 않고 실행합니다. 새 기능이 포함된 버전으로 업데이트하려면 사용자의 업데이트 요청에 따라 `-Update`를 붙입니다. 다운로드 경로와 임시 파일은 실행마다 분리되며 스크립트가 사용자 파일을 삭제하지 않습니다.

```powershell
# Release 정보만 확인: 다운로드·설치·앱 실행 없음
& .\install-byc-windows.ps1 -InspectOnly

# 지정 버전 설치 또는 업데이트
& .\install-byc-windows.ps1 -Version v1.0.46 -Update
```

위 버전은 명령 형식 예시입니다. 연결 기능이 포함된 Release를 사용하세요. 실제 설치는 최대 15분 기다리며, 시간 초과 시 기존 설치/승인 창을 확인하고 중복 실행하지 않습니다.

## 검증 범위

다운로드 선택·해시 검사·설치 실행 경로는 자동 회귀 검사로 확인합니다. 실제 EXE 설치와 SmartScreen 클릭은 아직 검증하지 않았습니다. 기존 로컬 플러그인은 개발 환경에서 프로젝트·노드 조회까지 확인했으며 실제 생성은 미검증입니다.

[ThreeMod 배포 저장소](https://github.com/Niceofer/ThreeMod)
