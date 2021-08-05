github의 코드분석중 CNN-SVM model, CNN-Softmax model을 비교하기 위해서 SVM과 Softmax을 비교함

![5](https://user-images.githubusercontent.com/53909511/128356321-0f93b87d-f377-4424-80c4-be7ee20223f3.PNG)


SVM과 Softmac는 동일하게 class의 score vector를 계산한다.  
##### 차이점은 f를 어떻게 해석하냐에 있다. ##### 
Softmax classifier는 score로 만족하지 않고 correct class가 항상 높은 확률을 가질 수 있도록 학습한다. 점수를 확률로 해석해서, correct class의 확률은 높아지도록 한다.   
반면에 SVM은 margin이 만족되면 score를 조정하지 않는다. class score로 해석해서 loss function은 correct class가 다른 class 보다 높은 점수를 얻도록 한다.   


SVM과 Softmax 사이의 성능 차이는 대개 매우 작으나, Softmax classifier는 score로 만족하지 않고 correct class가 항상 높은 확률을 가질 수 있도록 학습하나, SVM은 margin이 만족되면 score를 조정하지 않는다.  
SVM이 값변화에 둔감하다.  
