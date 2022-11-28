# BLOG GAME 생성 과정
1. 테마 fork 후 로컬에 clone하기

내가 고른 [테마](https://github.com/abhinavs/moonwalk)의 Github로 이동하여 내 repository로 fork한다. 이후 [Git&Github 포스트](https://clzlol.github.io/git-github)에 있는 git clone을 이용해 fork하여 내 repo에 불러온 파일들을 로컬로 복사한다.


2. jekyll 설치

이후 ruby를 설치한 후 터미널에서 다음 명령어를 실행해 Jekyll 설치를 진행한다.
```bash
gem install jekyll bundler
```


3. 포스트 작성

Markdown을 이용해 [다음](https://clzlol.github.io/google-analytics-%EC%B6%94%EA%B0%80)과 같은 post를 작성한다.


4. 댓글 추가

먼저 [Disqus](https://disqus.com/)에 가입하고 Universal Embed Code를 복사하여 _layouts 폴더 내의 post.html에 붙여넣기를 해준다. 이후 page.url과 page.identifier에 내 Git Blog의 주소와 닉네임을 적어준다. 그리고 _config.yml의 아래에 다음 코드를 추가해준다.

```markdown
comment:
  provider: "disqus"
  disqus:
    shortname: "clzlol"
```

마지막으로 댓글 기능을 추가할 post 파일에 아래의 코드를 추가해준다.

```markdown
comments: true
```


5. google analytics 추가

이것에 대한 자세한 과정은 [이 주소](https://clzlol.github.io/google-analytics-%EC%B6%94%EA%B0%80)에 나와있다.