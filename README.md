# keysburn.github.io

[Jekyll](https://jekyllrb.com/) + [Chirpy 테마](https://github.com/cotes2020/jekyll-theme-chirpy)로 만든 기술 블로그입니다.
`main` 브랜치에 push하면 GitHub Actions가 빌드 후 GitHub Pages(<https://keysburn.github.io>)로 자동 배포합니다.

## 글 쓰기

1. `_drafts/post-template.md`를 복사해 `_posts/YYYY-MM-DD-제목.md`로 저장합니다. (파일명의 제목 부분은 영문 kebab-case 권장 → URL이 `/posts/제목/`이 됩니다.)
2. front matter(`title`, `date`, `categories`, `tags`)를 채우고 본문을 작성합니다.
3. 이미지는 `assets/img/posts/`에 두고 `![설명](/assets/img/posts/파일명.png)`로 참조합니다.
4. 커밋 & push 하면 몇 분 안에 배포됩니다.

작성 중인 글은 `_drafts/`에 두면 배포되지 않습니다. (로컬에서 `--drafts` 옵션으로 미리보기 가능)

자세한 문법(프롬프트 박스, 파일명 표시, 수식, Mermaid 등): [Writing a New Post](https://chirpy.cotes.page/posts/write-a-new-post/)

## 로컬 미리보기

### Ruby가 설치된 경우

```bash
bundle install
bundle exec jekyll serve --livereload --drafts
```

### Docker만 있는 경우

```bash
docker run --rm -it -p 4000:4000 -v "$PWD":/srv/jekyll -w /srv/jekyll ruby:3.4 bash -c "bundle install && bundle exec jekyll serve -H 0.0.0.0 --livereload --drafts"
```

<http://localhost:4000> 에서 확인합니다.

## 주요 설정 (`_config.yml`)

- `title`, `tagline`, `description`: 블로그 이름/소개
- `avatar`: 사이드바 프로필 이미지
- `comments.provider`: 댓글 (`giscus` 권장 — <https://giscus.app> 에서 값 발급)
- `analytics`: Google Analytics 등
- `webmaster_verifications.google`: Google Search Console 인증 코드
