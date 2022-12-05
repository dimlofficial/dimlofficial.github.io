# DIML Homepage powered by Jekyll
Migration by [Eungbean Lee](https://eungbean.io)

## Useage

[*] 표시된 폴더를 주로 수정합니다.
```sh
.
├── _data
│   ├── assets.yml                  : css, js 정보
│   ├── news.yml                    : [*]메인화면 News 데이터
│   ├── patents_domestic.yml        : [*]특허-국내
│   ├── patents_international.yml   : [*]특허-국제
│   └── patents_ongoing.yml         : [*]특허-진행중
├── _includes                   : Jekyll html 컴포넌트
├── _layouts                    : Jekyll layout
├── assets                      : Jekyll css, js
├── downloads                   : Downloadable 파일 데이터
├── images                      : 각종 이미지
├── pages                       : Jekyll html pages
│   ├── alumni.html
│   ├── contact.html
│   ├── dataset.html
│   ├── introduction.html
│   ├── lecture.html
│   ├── photo.html
│   ├── postdoc.html
│   ├── professor.html
│   ├── projects.html
│   ├── pub_domesconf.html      : [*]논문-국내학회
│   ├── pub_domesjournal.html   : [*]논문-국내저널
│   ├── pub_intlconf.html       : [*]논문-국제학회
│   ├── pub_intljournal.html    : [*]논문-국제저널
│   ├── pub_patents.html        : [*]특허
│   ├── pub_patents_backup.html
│   └── research                : 과제관련
└── popups                      : 팝업관련 (현재사용안함)
```

## Procedure

#### 1. pages 업데이트
```sh
.
├── pages 
    ├── pub_domesconf.html      : [*]논문-국내학회
    ├── pub_domesjournal.html   : [*]논문-국내저널
    ├── pub_intlconf.html       : [*]논문-국제학회
    └─ pub_intljournal.html     : [*]논문-국제저널
```

#### 2. News update

```sh
.
├── _data 
    └─ news.html     : [*]메인화면 News 데이터
```

#### 3. Push
```sh
git add . && git commit -m "document update" && git push
```


## Toss Log
응빈 migration
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