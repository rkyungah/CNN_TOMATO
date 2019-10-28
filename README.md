## CNN project - tomato classification
<br>

### 개요
익지 않은 토마토에 존재하는 독성과, 토마토를 재배할 때 드는 노동을 간편화하기 위해 이 프로젝트를 진행하였다. 스토어팜 등 농작물 재배 시장이 커지고, 그에 따른 노동력이 필요하나 확충이 쉬이 되지 않는 상황에서 드론 등을 통해 입수한 이미지들을 CNN에 넣어 분류하면, 정확도가 높을 시 수확가능한 토마토를 고르는 과정에 드는 시간이 크게 감소할 수 있을 거라 예상한다.
우리는 모델에서 크게 초록색(익지 않은 토마토)와 붉은색(다 익은 토마토)를 분류했으며 그 중간 지점에 있는 토마토를 얼마나 정교하게 분류하는지를 확인했다. 줄기가 있는 토마토와 없는 토마토, 잘린 토마토 등 다양한 토마토 사진을 이용해 CNN 모델을 만들어 분류했다.
<br>
<br>

#### 이미지 수집
1) web crawling
   <p> 1. google image downloader (https://github.com/hardikvasa/google-images-download) </p>
   <p>2. bing image downloader (https://icrawler.readthedocs.io/en/latest/) </p>
<br>

#### CNN
tensorflow를 사용. 총 4개의 층을 쌓고 Same padding과 2X2 stride로 conv. <br>
optimizer = Adam
batch_size = 100

#### accuracy
정확도 :  0.95789474

   

