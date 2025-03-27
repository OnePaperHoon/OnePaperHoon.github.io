+++
date = '2025-03-28T07:11:57+09:00'
draft = false
title = 'Hugo 사용하면서 정리'
+++

## Make New Post
1. hugo new [path]/[name].md
2. 그리고 obisidian에서 작성

## hugo server -D
Live Server로 보면서 작성 가능 단점은 라이브 서버를 빌드 할 경우
public이라는 폴더가 생성된걸 깃허브에 올릴 경우 url이 꼬여서 페이지 로드가
안될수 있음

## categories =
블로그의 content 파일 구조는

```
├── content
│   └── posts
│       ├── OpenGL
│       │   └── \010What is OpenGL.md
│       ├── hugo.md
│       └── 공부정리.md
```

이렇게 되어 있는데 때문에 글을 정리 할때는 ctategories = [folder name] 으로  정리한다.

## Code Box
1. 앞으로의 코드 설명이나 구현코드를 올릴때는
```
이렇게 ```으로 구성된 코드 박스를 이용하거나
Vscode에서 PolaCode로 이미지화 시켜서 적용한다
```

![Code Box](/images/Hugo.png)

> Static/images폴더에 넣어둔 이미지를 찾아서 넣고싶다면 슬프게도 obisidian과  
> hugo에서의 경로 인식이 다르기 때문에 images폴더에 있는 것에 접근할때 
> static은 빼고 images/imagename.png 로 접근해야함