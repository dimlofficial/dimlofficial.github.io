todo:

/images/member 에 사진추가

상률이 토스받음

응빈이가 토스해줌

## Changelogs
---
### 21-03-04
* 메인화면 News 섹션 하드코딩 되어있는 곳을 Liquid Script로 Reformulation
  - ```_include/2-news_script.html``` 에 구현해 ```_include/2-news.html```에 삽입
  - ```_data/news.yml```에 해당 컨퍼런스 / 저널 입력

* Slide 추가
  - ```/images/Popup/{YYYY}-{MM}/Slide0.png``` 로 추가함
  - [TODO] liquid query로 구현 후 ```_data/popup.yml``` 에 데이터 저장하기
    - 일부 구현: ```_data/popup.yml```, ```_includes/popup.html``` 