# Fitness

[참고영상](https://youtu.be/KBpoBc98BwM?si=JYyjQZuUQLxoLbh4)

## 설치
```js
 "dependencies": {
    "@emotion/react": "^11.9.0",
    "@emotion/styled": "^11.8.1",
    "@mui/icons-material": "^5.6.1",
    "@mui/material": "^5.6.1",
    "react": "^18.0.0",
    "react-dom": "^18.0.0",
    "react-horizontal-scrolling-menu": "^2.7.1",
    "react-loader-spinner": "^6.0.0-0",
    "react-router-dom": "^6.3.0",
    "react-scripts": "5.0.1"
  },
```
## 주요기능
Home: 홈페이지를 구성하는 메인 페이지 컴포넌트입니다.<br />
HeroBanner, SearchExercises, Exercises 컴포넌트를 통해 페이지를 구성하고, 상태를 관리합니다.<br />
<br />
ExerciseDetail: 특정 운동에 대한 상세 정보 페이지를 나타내는 컴포넌트입니다.<br />
Detail 컴포넌트로 운동의 세부 정보를 표시하고, ExercisesVideos와 SimilarExercises 컴포넌트로 해당 운동에 대한 비디오 및 유사한 운동을 표시합니다.<br />
<br />
Navbar: 네비게이션 바 컴포넌트입니다.<br />
Link를 사용하여 홈페이지로 이동할 수 있는 로고와 네비게이션 링크를 제공합니다.<br />
<br />
Loader: 로딩 상태를 표시하는 간단한 로더 컴포넌트입니다.<br />
react-loader-spinner 라이브러리를 사용하여 무한 스핀을 표현하고 있습니다.<br />
<br />
HorizontalScrollbar: 수평 스크롤바를 제공하는 컴포넌트입니다.<br />
react-horizontal-scrolling-menu를 사용하여 좌우 화살표로 스크롤 가능한 아이템들을 표시합니다.<br />
<br />
HeroBanner: 홈페이지 상단에 위치한 히어로 배너 컴포넌트입니다.<br />
사진, 제목, 부제목, 설명 텍스트 등을 포함한 페이지의 주요 내용을 나타냅니다.<br />
<br />
ExercisesVideo: 운동 비디오를 표시하는 컴포넌트입니다.<br />
YouTube API를 사용하여 동적으로 비디오 리스트를 가져와 표시합니다.<br />
<br />
Exercises: 운동 목록을 표시하고 페이지네이션을 제공하는 컴포넌트입니다.<br />
각 운동은 ExerciseCard 컴포넌트로 표시됩니다.<br />
<br />
ExerciseCard: 각 운동에 대한 간단한 정보와 링크를 제공하는 컴포넌트입니다.<br />
Link를 사용하여 개별 운동 페이지로 이동할 수 있는 링크를 제공합니다.<br />
<br />
Detail: 개별 운동 페이지에서 해당 운동의 세부 정보를 나타내는 컴포넌트입니다.<br />
운동의 이름, 설명, 이미지 등을 표시하며, 세부 정보는 BodyPart, Target, Equipment 세 가지로 나누어 표시합니다.<br />
<br />
BodyPart: 운동 부위를 선택할 수 있는 버튼 컴포넌트입니다.<br />
선택된 부위는 페이지의 운동 목록을 필터링하는 데 사용됩니다.<br />
<br />
SearchExercises: 홈페이지에서 운동 검색과 관련된 기능을 담당하는 컴포넌트입니다.<br />
TextField를 사용하여 검색어를 입력할 수 있고, 검색 버튼을 눌러 검색을 수행합니다.<br />
수평 스크롤바로 운동 부위 목록을 표시하고, 선택된 부위에 따라 페이지의 운동 목록을 필터링합니다.<br />
<br />
SimilarExercises: 특정 타겟 근육이나 운동 장비에 대한 비슷한 운동을 표시하는 컴포넌트입니다.<br />
HorizontalScrollbar 컴포넌트를 사용하여 비슷한 운동들을 수평으로 스크롤하여 표시합니다.<br />
<br />
