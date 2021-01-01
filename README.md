# Latitude-and-longitude-of-metropolitan-subway
----------------------
1. 수도권 지하철역 각각의 이름이 담긴 엑셀 파일을 input으로 넣는다.
input data : 서울교통공사 공공데이터개방 부분에서 아래 url의 엑셀 파일 (2020-11-10기준)
http://www.seoulmetro.co.kr/kr/board.do?menuIdx=551&bbsIdx=2210979

2. get_location_v2.py의 실행 결과로 지하철 역 별 위도&경도를 엑셀파일로 출력한다.

3. 2번의 결과로 나온 결과값의 오류를 찾기 위해 point_location.py를 사용한다.
지도 위에 점을 찍고 역명을 표기해줌으로써 위치 오류를 찾을 수 있다. -> issue의 오류

issue: 역 이름 형태가 인식불가 또는 동명의 역이 존재할 경우 값이 None 또는 쌩뚱맞은 위치의 역 정보가 가져와질 수 있다.
-> html로 나타내어진 지도에 point를 찍어서 잘못된 위치의 역을 확인 후 수기로 수정

<img width="800" src="https://user-images.githubusercontent.com/57093610/103170791-72953580-488a-11eb-9d8e-f46aba529747.PNG">
