# KVELOPER

GitHub Pages의 Jekyll로 자동 빌드되는 다국어 문서 사이트입니다. 내용을 수정하고 배포 브랜치에 커밋·푸시하면 반영됩니다. 수동 컴파일은 필요하지 않습니다.

- `eng.md`: 영어, 기본 홈(`/`)
- `kor.md`: 한국어(`/kor.html`)
- `jpn.md`: 일본어(`/jpn.html`)

각 파일의 상단 `---` 설정은 유지하고 아래 Markdown 본문을 수정하세요. 각 언어의 내용은 별도로 관리합니다. 상단 이미지 버튼으로 언어를 전환하며 외부 번역 서비스를 사용하지 않습니다.

한국어·영어는 Pretendard, 일본어는 Pretendard JP를 사용합니다. 각 폰트의 Medium(500)과 ExtraBold(800) WOFF2만 포함하며, 페이지별로 필요한 폰트만 불러옵니다. 배포 시 폰트 라이선스는 `assets/fonts/`에 함께 포함됩니다.

GitHub 저장소 Settings → Pages에서 Deploy from a branch 및 배포 브랜치의 /(root)를 사용하세요.
