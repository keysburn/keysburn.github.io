---
title: 기술 블로그를 시작합니다
date: 2026-09-24 21:00:00 +0900
categories: [Blog, Setup]
tags: [jekyll, chirpy, github-pages]
description: Jekyll + Chirpy 테마 + GitHub Pages로 기술 블로그를 세팅했습니다.
---

기술 블로그를 시작합니다. 개발하며 배운 것, 삽질한 것, 정리해두고 싶은 것들을 기록할 예정입니다.

## 블로그 구성

| 항목 | 내용 |
| --- | --- |
| 정적 사이트 생성기 | [Jekyll](https://jekyllrb.com/) |
| 테마 | [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) |
| 호스팅 | GitHub Pages |
| 배포 | GitHub Actions (push 시 자동 배포) |

## 코드 하이라이트 테스트

```python
def hello(name: str) -> str:
    return f"Hello, {name}!"

print(hello("world"))
```

```bash
bundle exec jekyll serve
```
{: file="terminal" }

> 팁 박스는 이렇게 씁니다.
{: .prompt-tip }

> 주의가 필요할 땐 이렇게 씁니다.
{: .prompt-warning }
