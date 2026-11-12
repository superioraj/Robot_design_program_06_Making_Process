# ROBOT BUILD LOG 1.2

사진 6장으로 로봇 제작 과정을 기록하고 A4 세로 PDF 보고서로 출력하는 GitHub Pages용 정적 웹 앱입니다.

## 카메라
- `[ + PHOTO ]` 영역을 누르면 `navigator.mediaDevices.getUserMedia()`로 브라우저 내부 카메라 미리보기를 엽니다.
- 후면 카메라를 우선 요청하며, `[촬영]` 또는 Space 키로 캡처합니다.
- 카메라 권한이 거부되면 주소창의 카메라 아이콘에서 허용 후 다시 실행합니다.
- 카메라는 HTTPS(GitHub Pages) 또는 localhost에서만 작동합니다. `file://`로 직접 열면 브라우저 보안 정책상 실행되지 않을 수 있습니다.
- 실시간 카메라를 지원하지 않는 기기에는 `카메라 앱으로 촬영` 대체 버튼을 표시합니다.
- `[사진 선택]`은 계속 기기에 저장된 파일을 업로드합니다.

## PDF 표선
- 기본 정보 표, 제작 단계 카드, 사진 프레임, 제작 정리 상자의 선을 모두 `0.3mm solid #000`으로 통일했습니다.
- `border-collapse: collapse`, `print-color-adjust: exact`, `box-shadow: none`을 적용하여 브라우저 인쇄에서 선 굵기가 달라 보이는 현상을 줄였습니다.

## 실행
카메라를 사용하려면 GitHub Pages에 배포하거나 localhost 서버에서 실행하세요. GitHub Pages에서는 `robot-build-report.html`을 `index.html`로 이름을 바꿔 저장소 루트에 올립니다.
