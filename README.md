# KVELOPER — 정적 개발자 포트폴리오

GitHub Pages의 Jekyll로 빌드되는 사이트입니다. 현재 8개 카드는 교체용 예시입니다.

## 프로젝트 추가

`post/` 바로 아래에 `.md` 파일을 추가하세요. 파일명 사전순으로 정렬되므로 `01-`, `02-`처럼 자릿수를 맞춘 접두사를 권장합니다.

```yaml
---
title: "내 프로젝트"
subtitle: "프로젝트 한 줄 소개"
category: "WEB GAME"
image: /assets/images/my-project.png
github: https://github.com/kveloper/my-project
play: /games/my-project/index.html
---

## 소개

프로젝트 설명을 Markdown으로 작성합니다.
```

`image`는 정사각형 썸네일 경로입니다. 생략하면 기본 이미지가 표시됩니다. `github`, `play`는 선택 사항이며, 설정한 링크만 상세 페이지에 버튼으로 표시됩니다. 외부 HTTPS 게임 주소도 지원합니다.

이미지는 `assets/images/`, 웹게임 파일은 `games/게임명/`에 저장하세요. 게임 내부 파일 참조는 상대 경로를 사용하세요. 카드 클릭 시 Markdown 상세 페이지로 이동하고, 상세 페이지에서 게임·저장소 링크를 엽니다.

## 배포 및 로컬 실행

GitHub 저장소 Settings → Pages에서 **Deploy from a branch**를 선택하고 사이트 파일을 올린 브랜치의 **/(root)**를 지정하세요. Markdown 변경 사항은 GitHub Pages가 자동 빌드합니다.

Ruby와 Bundler가 설치되어 있다면 다음 명령으로 로컬에서 확인할 수 있습니다.

```sh
bundle install
bundle exec jekyll serve
```

`http://localhost:4000`을 엽니다. HTML 파일을 직접 열거나 일반 정적 서버를 사용하면 Liquid 템플릿이 처리되지 않으므로 Jekyll 빌드가 필요합니다.

`_config.yml`의 사이트 제목·설명을 수정하세요. 프로젝트 저장소 주소에 배포할 때는 `baseurl: "/저장소명"`을 지정하세요. 로고와 GitHub 계정 링크는 `index.html`, `_layouts/project.html`에서 변경합니다.

## 디자인

카드는 간격 없이 정사각형으로 채워지며 화면 너비에 따라 열과 행 수가 변경됩니다. 모바일 기본 2열, 340px 미만 1열입니다. 모든 글은 스크롤로 확인할 수 있습니다. 마우스 hover와 키보드 focus 시 흰 테두리와 어두워지는 효과를 제공하며 동작 줄이기 설정을 지원합니다.

제공된 `Windows_TTF` 폴더의 Light·Medium 폰트를 `assets/fonts/`에 복사하여 사용합니다. 원본 폴더는 보존합니다.
