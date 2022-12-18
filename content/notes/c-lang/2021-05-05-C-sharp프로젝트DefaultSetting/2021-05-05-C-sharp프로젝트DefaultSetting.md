---
title: "C# 프로젝트 Default Setting" # Title of the blog post.
date: 2021-05-05 # 월, 일은 꼭 2자리로 작성 (ex. 12-08)
description: "Article description." # Description used for search engine. (검색엔진을 위한 설명)
featured: false # Sets if post is a featured post, making appear on the home page side bar. (feature는 하나만 하던가 쓰지 말자)
draft: false # Sets whether to render this page. Draft of true will not be rendered. (set false 해야 포스팅 된다)
toc: false # Controls if a table of contents should be generated for first-level links automatically. (페이지 상단 목차 기능인듯함)
# menu: main # 열면 사이트 상단에 제목이 나타난다.
usePageBundles: false # Set to true to group assets like images in the same folder as this post. (?)
#featureImage: "/images/path/file.jpg" # Sets featured image on blog post. (메인 이미지)
featureImageAlt: 'Description of image' # Alternative text for featured image.
featureImageCap: 'This is the featured image.' # Caption (optional).
#thumbnail: "/images/path/thumbnail.png" # Sets thumbnail image appearing inside card on homepage. (썸네일 이미지)
#shareImage: "/images/path/share.png" # Designate a separate image for social media sharing.
codeMaxLines: 10 # Override global value for how many lines within a code block before auto-collapsing.
codeLineNumbers: true # Override global value for showing of line numbers within code block.
#figurePositionShow: true # Override global value for showing the figure label.
#categories 는 한 개만 달고, 많이 늘리지 않도록.
categories:
  - c/c#
tags:
  - c#
# comment: false # Disable comment if false.
---

## Tools

- Just Color Picker : Screen 상에서 색상 RGB 값 따는 프로그램

## Form1

- StartPosition : CenterScreen
    - 폼이 처음 나타날 때 해당 폼의 위치를 결정
    
- AutoScaleMode : None
    - 화면 해상도나 글꼴이 변경될 때 폼이나 컨트롤의 크기가 조정되는 방식을 결정합니다.
    - 실행 환경 변경 시 레이아웃이 깨지는 문제를 방지할 수 있다.
    - Dpi : 디스플레이 해상도를 기준으로 크기를 제어합니다. 일반적인 해상도는 96 및 120DPI입니다.
    - Font : 클래스에서 사용하는 글꼴(일반적으로 시스템 글꼴)의 크기를 기준으로 크기를 제어합니다.
    - Inherit : 클래스의 부모 크기 조정 모드에 따라 크기를 제어합니다. 부모가 없는 경우 자동 크기 조정을 사용하지 않습니다.
    - None : 자동 크기 조정을 사용하지 않습니다.
- Font : 뭐든 정하고 시작 (기본 폰트는 아니지만 Noto Sans 추천이 많다.)
- FormBorderStyle : None
    - 폼의 테두리 및 제목 표시줄의 모양과 동작을 나타냅니다.
    - None이 예쁘기는 한데 불편하니까 default라기 보다는 상황에 따라 설정
    - None으로 변경하면 종료버튼이나 사이즈 조절 버튼이 사라져서 만들어 줘야함