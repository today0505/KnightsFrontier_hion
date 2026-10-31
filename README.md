# 내 블로그 (GitHub Pages + Jekyll)

## 1. 내 정보로 바꾸기
- `_config.yml` → `author`, `github`, `url`, `title`, `tagline`
- `about.md` → 자기소개 내용
- `assets/css/style.css` → 상단의 `:root` 색상 값(`--blue`, `--lime` 등)을 바꾸면 분위기가 바뀝니다.
- 프로필 사진 → `assets/img/profile.jpg`로 올리면 소개 페이지에 자동으로 나옵니다. (정사각형 권장)
- 카테고리 색상 → `assets/css/style.css`의 `.c-dev`, `.c-ctf` … 항목

## 2. 배포하기
1. GitHub에서 **`<내아이디>.github.io`** 이름의 Public 저장소를 만듭니다.
2. 이 폴더의 파일을 모두 올립니다. (`.gitignore`, `_data` 등 점/밑줄 폴더 포함)
3. 저장소 **Settings → Pages**에서 Source를 *Deploy from a branch*, Branch를 `main` / `(root)`로 선택합니다.
4. 1~2분 뒤 `https://<내아이디>.github.io`에서 확인합니다.

## 3. 글 쓰기
`_posts/YYYY-MM-DD-제목.md` 파일을 만들고 아래 형식으로 시작합니다.

```
---
layout: post
title: "글 제목"
categories: [ctf]
---
본문
```

`categories`에 넣을 수 있는 값: `dev`, `ctf`, `bugbounty`, `writing`, `papers`, `contests`

## 4. 로컬에서 미리 보기 (선택)
```
bundle install
bundle exec jekyll serve
```
