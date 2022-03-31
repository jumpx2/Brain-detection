# Brain-detection


```python
# !git clone https://www.github.com/matterport/Mask_RCNN
# model git clone으로 받아오기
# !git clone https://github.com/atakanady/brain-tumor
# brain tumor 데이터 clone
# !pip install pycocotools
# !pip install -r requirements.txt
# !python3 setup.py install
```


```python
Tensorflow 1.x 버전 활용
- Tensorflow 2.x 버전 오류를 다 잡지 못해 제출 기간 맞추기위해 tensorflow 1.x cpu활용
- cpu로 모델 적용이기에 1epochs 당 40~50분 소요 
- annotation은 데이터셋에 정의가 되어있음
- annotation site = https://www.robots.ox.ac.uk/~vgg/software/via/via.html
이 사이트에서 annotaion 사진마다 각각 정해줄 수 있고 json으로 파일도 만들기 가능
```
```
결과
- dataset에서 annotation을 하고 model에 적용 함 
- 생각한 만큼 결과가 잘 나옴
```

```
## 느낀점 
- 버전 오류에 상당히 고난을 겪음
- 이미지처리는 무조건 gpu를 사용해야 한다라고 느낌
- annotation이 아무리 정확하더라고 모델이 잘 찾지 못하기도 함
```
![brain](https://user-images.githubusercontent.com/81940655/160998163-3b1ece1d-7058-4f10-85eb-5b4f43d86384.gif)

