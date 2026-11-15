# Igunis — 기술 블로그와 포트폴리오

GitHub Pages와 Jekyll로 만든 개인 사이트입니다. Markdown으로 글을 추가할 수 있습니다.

## 글 쓰기

`_posts/YYYY-MM-DD-english-slug.md` 파일을 만들고 다음 형식으로 작성합니다.

```md
---
layout: post
title: "글 제목"
description: "목록에 표시할 한 줄 설명"
date: 2026-11-16 00:00:00 +0900
category: Notes
tags: [V8, JavaScript]
---

본문을 Markdown으로 작성합니다.
```

공개 전 초안은 `_drafts/`에 저장할 수 있습니다. `writing/index.html`이 공개된 글을 자동으로 나열합니다.

## 내용 수정

- 첫 화면: `index.html`
- 자기소개: `about/index.html`
- 프로젝트: `projects/index.html`
- 디자인: `assets/css/main.css`
- 사이트 제목과 주소: `_config.yml`

실제 프로젝트를 추가할 때는 목표, 본인이 맡은 일, 결과와 확인 가능한 링크를 함께 적는 것을 권장합니다.

## 배포

GitHub 저장소의 **Settings → Pages → Build and deployment**에서 **Deploy from a branch**, `main`, `/(root)`를 선택합니다. 이후 `main`에 푸시하면 `https://igunis.github.io/`에 반영됩니다.

로컬 미리보기에는 Ruby가 필요합니다. `gem install jekyll -v 3.10.0`과 `gem install kramdown-parser-gfm -v 1.1.0`을 실행한 뒤, 저장소에서 `jekyll serve`를 실행하고 `http://127.0.0.1:4000/`을 열면 됩니다. (RubyGems의 실행 파일 디렉터리가 `PATH`에 있어야 합니다.)
