# 'Visual Studio'에서 OpenCV를 활용하는 환경 구축

1.OpenCV download를 통해서 다운을 받고 실행을 하여 파일을 생성<br>
2.C드라이브로 생성한 opencv파일 이동<br>
3.visual studio를 열어 콘솔 앱 c++로 c++코드 작성 환경 만들기<br>

## Visual Studio 환경 구축
- 속성 설정시 맨위 구성이 모든 구성으로 되었는지 확인
4.젤 위에 <b>프로젝트 탭</b>에서 <b>속성</b> 창을 클릭후 설정 편집<br>
5.C/C++ 탭에 일반 선택후 추가 포함 디렉터리 부분 편집<br>
-> C:\opencv\build\include<br>
<img src="https://github.com/cheol333/use_openCV/blob/main/set_img/set1.png?raw=true" width="500px" height="300px">
6.링커 탭에 일반 -> 추가 라이브러리 디렉터리 편집<br>
-> C:\opencv\build\x64\vc16\lib<br>
<img src="https://github.com/cheol333/use_openCV/blob/main/set_img/set2.png?raw=true" width="500px" height="300px">
7. 링커 탭에 입력 -> 추가 종속성 편집
-> opencv_world490d.lib<br>
-> opencv_world490.lib<br>
<img src="https://github.com/cheol333/use_openCV/blob/main/set_img/set3.png?raw=true" width="500px" height="300px">
<hr>
8.윈도우 검색으로 '시스템 환경 변수 편집' 입력 후 편집<br>
-> path 부분에 들어가서 'C:\opencv\build\x64\vc16\bin' 추가 후 저장<br>
<hr>
9.코드로 돌아와서 'C:\opencv\sources\samples\cpp' 여기에 있는 예제 파일을 가지고 실행 해보기<br>
10.이미지를 사용하려면 오른쪽 솔루션 탐색기에서 오른쪽 키를 눌러 '파일 탐색기에서 폴더 열기' 누른 후 이미지 파일 넣어주기<br>
<img src="https://github.com/cheol333/use_openCV/blob/main/set_img/set5.png?raw=true" width="500px" height="300px">
11.다시 위에 열었더 속성창을 열어 구성속성 탭에 디버깅-> 명령인수를 사진 파일 이름으로 변경 ex)test.jpg<br>
<img src="https://github.com/cheol333/use_openCV/blob/main/set_img/set4.png?raw=true" width="500px" height="300px">
<hr>
## OpenCV 중 edge 활용해보기
- 원본 이미지
<img src="https://github.com/cheol333/use_openCV/blob/main/test.jpg?raw=true" width="500px" height="300px">
- edge 적용 후 결과
<img src="https://github.com/cheol333/use_openCV/blob/main/edge_result.png?raw=true" width="500px" height="300px">
