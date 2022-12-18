---
title: "JUnit5:assertThrows" # Title of the blog post.
date: 2022-02-26 # 월, 일은 꼭 2자리로 작성 (ex. 12-08)
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
  - test
tags:
  - test
# comment: false # Disable comment if false.
---

### 예제

```java
    @Test
    public void 중복_회원_예외() throws Exception {
        //Given
        Member member1 = new Member();
        member1.setName("spring");

        Member member2 = new Member();
        member2.setName("spring 1"); // 같은 이름으로 중복 회원가입

        //When

        memberService.join(member1);
        IllegalStateException e = assertThrows(IllegalStateException.class,
                () -> memberService.join(member2));//예외가 발생해야 한다.
        //assertThat(e.getMessage()).isEqualTo("이미 존재하는 회원입니다.");
    }
```

- assertThrows( 발생해야 할 Exception, 검사할 람다식);
- Exception가 발생하지 않아도, 예상되지 않은 Exception이 발생해도 Test가 Fail 난다.
