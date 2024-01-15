# Fitness
<img width="100%" src="https://github.com/yunyoungsik/fitness/blob/main/src/assets/tumbnail.png?raw=true" />
Fitness Club은 다양한 운동 정보를 탐색할 수 있는 기능을 제공합니다.<br />
사용자는 원하는 운동을 검색하거나, 특정 부위 또는 운동 기구에 따라 쉽게 필터링하여 필요한 정보를 얻을 수 있습니다.<br />
   
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
- Home<br />
홈페이지를 구성하는 메인 페이지 컴포넌트입니다.<br />
HeroBanner, SearchExercises, Exercises 컴포넌트를 통해 페이지를 구성하고, 상태를 관리합니다.<br />
<br />
- ExerciseDetail<br />
특정 운동에 대한 상세 정보를 표시하는 페이지 컴포넌트<br />
URL Parameter에서 운동 ID 가져오기: useParams 훅을 사용하여 URL에서 운동 ID를 가져옵니다.<br />
데이터 Fetch 및 상태 관리: useEffect 훅을 사용하여 페이지가 로드될 때 필요한 데이터를 가져와 상태에 저장합니다.<br />
세부 정보 표시: Detail 컴포넌트를 통해 운동의 세부 정보를 표시합니다.<br />
운동 비디오 표시: ExercisesVideos 컴포넌트를 통해 YouTube에서 검색된 운동 관련 비디오를 표시합니다.<br />
유사한 운동 표시: SimilarExercises 컴포넌트를 통해 타겟 근육 및 장비에 따라 유사한 운동을 표시합니다.<br />
스크롤 최상단 이동: 페이지 로드 시에 스크롤을 페이지 상단으로 이동시킵니다.<br />
<br />
- exerciseOptions, youtubeOptions, fetchData<br />
exerciseOptions: ExerciseDB API 및 빠른 API 키를 사용하여 운동 데이터를 가져오기 위한 옵션입니다.<br />
youtubeOptions: YouTube 검색 및 다운로드 API 키를 사용하여 YouTube에서 운동 관련 비디오를 검색하기 위한 옵션입니다.<br />
fetchData 함수: 주어진 URL과 옵션을 사용하여 데이터를 비동기적으로 가져오는 함수입니다. fetch를 사용하여 데이터를 가져온 후 JSON으로 변환하여 반환합니다.<br />
<br />
- Navbar<br />
네비게이션 바 컴포넌트입니다.<br />
Link를 사용하여 홈페이지로 이동할 수 있는 로고와 네비게이션 링크를 제공합니다.<br />
<br />
- Loader<br />
로딩 상태를 표시하는 간단한 로더 컴포넌트입니다.<br />
react-loader-spinner 라이브러리를 사용하여 무한 스핀을 표현하고 있습니다.<br />
<br />
- HorizontalScrollbar<br />
수평 스크롤바를 제공하는 컴포넌트입니다.<br />
react-horizontal-scrolling-menu를 사용하여 좌우 화살표로 스크롤 가능한 아이템들을 표시합니다.<br />
<br />
- HeroBanner<br />
홈페이지 상단에 위치한 히어로 배너 컴포넌트입니다.<br />
사진, 제목, 부제목, 설명 텍스트 등을 포함한 페이지의 주요 내용을 나타냅니다.<br />
<br />
- ExercisesVideo<br />
운동 비디오를 표시하는 컴포넌트입니다.<br />
YouTube API를 사용하여 동적으로 비디오 리스트를 가져와 표시합니다.<br />
<br />
- Exercises<br />
운동 목록을 표시하고 페이지네이션을 제공하는 컴포넌트입니다.<br />
각 운동은 ExerciseCard 컴포넌트로 표시됩니다.<br />
<br />
- ExerciseCard<br />
각 운동에 대한 간단한 정보와 링크를 제공하는 컴포넌트입니다.<br />
Link를 사용하여 개별 운동 페이지로 이동할 수 있는 링크를 제공합니다.<br />
<br />
- Detail<br />
개별 운동 페이지에서 해당 운동의 세부 정보를 나타내는 컴포넌트입니다.<br />
운동의 이름, 설명, 이미지 등을 표시하며, 세부 정보는 BodyPart, Target, Equipment 세 가지로 나누어 표시합니다.<br />
<br />
- BodyPart<br />
운동 부위를 선택할 수 있는 버튼 컴포넌트입니다.<br />
선택된 부위는 페이지의 운동 목록을 필터링하는 데 사용됩니다.<br />
<br />
- SearchExercises<br />
홈페이지에서 운동 검색과 관련된 기능을 담당하는 컴포넌트입니다.<br />
TextField를 사용하여 검색어를 입력할 수 있고, 검색 버튼을 눌러 검색을 수행합니다.<br />
수평 스크롤바로 운동 부위 목록을 표시하고, 선택된 부위에 따라 페이지의 운동 목록을 필터링합니다.<br />
<br />
- SimilarExercises<br />
특정 타겟 근육이나 운동 장비에 대한 비슷한 운동을 표시하는 컴포넌트입니다.<br />
- HorizontalScrollbar<br />
컴포넌트를 사용하여 비슷한 운동들을 수평으로 스크롤하여 표시합니다.<br />
<br />
