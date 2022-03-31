# Book-Review-App
도서 리뷰 안드로이드 앱

#### 인터파크 API를 활용해 도서 목록을 보거나, 도서 리뷰를 작성하 저장할 수 있는 도서 리뷰 앱 입니다.
### Blog
* <https://hwayomingdlog.tistory.com/247>
* <https://hwayomingdlog.tistory.com/248>
* <https://hwayomingdlog.tistory.com/249>
* <https://hwayomingdlog.tistory.com/251>
* <https://hwayomingdlog.tistory.com/252>
</br>

## 주 기능
### 베스트셀러
* 인터파크에서 제공하는 실시간 베스트셀러 목록을 확인 할 수 있습니다.

### 검색 히스토리
* 검색 키워드를 검색창에 입력해서 관련 도서 목록을 찾아 볼 수 있습니다.
* 이전에 검색한 키워드들이 저장되며, 키워드를 클릭해 재검색 할 수 있습니다.
* 검색 히스토리를 X 버튼을 클릭해 삭제 할 수 있습니다.

### 도서 리뷰
* 도서 목록에서 특정 도서를 클릭해 상세 정보를 확인 할 수 있습니다.
* 상세 정보 하단의 입력창을 통해 해당 도서에 관해 리뷰를 남기고 저장할 수 있습니다.
</br>

## 활용 기술
* Room Database - Room 데이터베이스 구성요소인 Entities, DAO, AppDatabase를 만들어서 검색 히스토리와 도서 리뷰를 앱 내부 저장소에 저장하였습니다.
* Retrofit2 - 인터파크 API를 활용해 서버에 저장된 데이터를 받아오기 위해 Retrofit2 라이브러리를 활용하였습니다.</br>Data class를 정의하여 데이터 모델을 만들고 DTO(Data Transfer Object)를 만들어 JSON 타입을 변환해서 key 값을 직렬화하여 지정한 property에 담기도록 하였습니다. </br>검색 결과를 가져오고 베스트셀러 목록을 가져오는 통신을 정의하는 서비스 interface를 정의했습니다.
* Glide - 서버에서 불러온 도서 이미지 URL을 사용해서 ImageView에 도서 이미지를 띄우기 위해 Glide 라이브러리를 사용했습니다.
* ConstraintLayout - ConstraintLayout의 Chain을 이용하여 View들의 위치를 설정하였습니다.
* RecyclerView - 도서 목록을 보여주기 위해 RecyclerView를 활용했습니다. </br>ListViewAdapter를 상속받아 DiffUtil을 통한 데이터 업데이트가 이뤄지도록 구현하였습니다.
</br>

***
<img src="/img/img0.png" width="300px" height="600px" title="" alt=""></img>
<img src="/img/img1.png" width="300px" height="600px" title="" alt=""></img>
<img src="/img/img2.png" width="300px" height="600px" title="" alt=""></img>
<img src="/img/img3.png" width="300px" height="600px" title="" alt=""></img>
<img src="/img/img4.png" width="300px" height="600px" title="" alt=""></img>
<img src="/img/img5.png" width="300px" height="600px" title="" alt=""></img>
<img src="/img/img6.png" width="300px" height="600px" title="" alt=""></img>
<img src="/img/img7.png" width="300px" height="600px" title="" alt=""></img>
