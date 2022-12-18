---
title: "C# panel" # Title of the blog post.
date: 2020-10-21 # 월, 일은 꼭 2자리로 작성 (ex. 12-08)
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

## 1. TableLayoutPanel

## 2. Panel

- TableLayoutPanel 으로 구도 잡고 위에 Panel 올려줘야 도구(controller? 컴포넌트?)들 올라감
- 재생버튼같은거 달려있는데 부모 컨테이너에 도킹 뭐지? 도킹이 뭐지?

## 3. 도킹

- TableLayoutPanel 에 Panel 놓고 도킹하니까 쫙 퍼지면서 Layout크기만큼 쭉 커진다.