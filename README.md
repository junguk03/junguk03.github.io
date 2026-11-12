# junguk03.github.io

Hugo로 만든 포트폴리오 + 블로그입니다.

## 로컬에서 보기

```bash
brew install hugo
hugo server        # http://localhost:1313
```

## 새 글 쓰기

```bash
hugo new blog/글-주소.md   # archetypes/blog.md 양식으로 생성 (draft: true)
hugo server -D             # 초안까지 미리보기
```

다 쓰면 파일 맨 위 `draft: true`를 지우거나 `false`로 바꾼 뒤 push 하면 공개돼요.

## 프로젝트·활동 수정

`data/projects.yaml`만 고치면 Home과 Projects 페이지에 같이 반영돼요.

| 키 | 내용 |
| --- | --- |
| `studying` | 공부 중인 PortSwigger 진행률 (`done` / `total`, `updated` 날짜도 같이 고치기) |
| `projects` | 주요 프로젝트 카드 |
| `exploits` | 워게임 익스플로잇 코드 목록 |
| `activities` | 대회·활동 |
| `others` | 기타 프로젝트 (Projects 페이지 맨 아래에 짧은 설명만) |

## 배포

1. GitHub `junguk03.github.io` 저장소에 이 폴더를 push (주소: https://junguk03.github.io/)
2. 저장소 Settings → Pages → Build and deployment → Source를 **GitHub Actions**로 선택
3. 이후 main에 push 할 때마다 `.github/workflows/hugo.yml`이 자동으로 빌드·배포
