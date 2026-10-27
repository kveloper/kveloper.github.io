# KVELOPER

`main.md`를 기본 홈(`/`)에 표시하는 GitHub Pages 사이트입니다.

`main.md` 상단의 `---` 설정은 유지하고 아래 Markdown 본문을 수정한 뒤 배포 브랜치에 커밋·푸시하면 Jekyll이 자동으로 빌드합니다. 수동 컴파일은 필요하지 않습니다.

사이트 이름은 `_config.yml`의 `title`에서 변경합니다. 파비콘은 `favicon.ico`를 사용합니다.

## 문서 탭

`_posts/YYYY-MM-DD-이름.md` 파일 하나가 타이틀 아래의 이동 버튼 하나에 대응합니다. `title`은 버튼 이름이며 `order` 숫자로 순서를 정합니다. 메인 버튼은 항상 첫 번째입니다. 예시 문서 3개는 자유롭게 수정하거나 삭제하세요.

```yaml
---
title: 새 문서
order: 4
---
```

파일명에는 오늘 또는 이전 날짜를 사용하세요. 미래 날짜 문서는 아직 표시되지 않습니다. 문서 상단에는 제목이 자동 표시되므로 본문에서 같은 H1을 반복할 필요는 없습니다.

폰트는 Pretendard Medium(500)과 ExtraBold(800) WOFF2를 사용하며, 라이선스는 `assets/fonts/Pretendard-LICENSE.txt`에 포함되어 있습니다.

GitHub 저장소 Settings → Pages에서 Deploy from a branch 및 배포 브랜치의 /(root)를 사용하세요.
