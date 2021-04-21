# - 기계학습 개념 정리하기

구글에서 제공하는 머신러닝 정리 사이트
https://developers.google.com/machine-learning/crash-course?hl=ko

**1. 편향과 분산**
https://www.opentutorials.org/module/3653/22071

**2. supervised와 unseperviesed**
- training data로 label을 요구하느냐 그렇지 않느냐

**3. ROC 커브**
- https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc?hl=ko

**4. Precision, Recall (정밀도, 재현)**
- https://developers.google.com/machine-learning/crash-course/classification/precision-and-recall

**5. 베이즈 정리? 머신러닝 맥락에서 어떤 유용함?**
- 프린트 참고
- 사전에 알고 있는 지식을 통해 사후 확률을 계산할 수 있다.
- 이러한 방법이 훨씬 정확하고 사전에 가지고 있는 데이터를 통해서 정보를 얻고 새로운 데이터에 대한 결과를 얻는 머신러닝에 적합하다.

**6. naive Bayes는 왜 naive 하냐?**
- text mining에서는 practical할진 몰라도 보통은 naive하다고 여겨진다.
- 실제 세계에서 찾아보기 힘든 가정을 깔고 있기 때문이다.
- 조건부 확률은 각 변수들마다 완전 독립적이다라는 가정을 깔고 가는데 이는 실세 세계에서 나타날 수 없기 때문이다.

7. L1, L2 regularization의 차이점
- L1은 다수의 가중치를 0으로 만들어 줄 수 있기 때문에 메모리를 차지 하지않아도 되고 모델의 노이즈도 줄어들어서 유용함
- https://developers.google.com/machine-learning/crash-course/regularization-for-sparsity/l1-regularization

8. 딥러닝은 무엇이고 머신러닝과 무엇이 다른가?
- 딥러닝은 머신러닝의 한 부분이다. 머신러닝과 달리 딥러닝은 깊은 인공신경망으로 이루어져 있으며 이 인공신경망을 통해 데이터의 특징들을 학습하게 된다.

9. generative한 모델과 discriminative한 모델의 차이점은 무엇인가?
- generative model은 데이터의 카테고리를 학습하지만
- discriminative model은 서로다른 데이터의 카테고리 사이의 거리를 학습한다.
- 일반적으로 discriminative model이 generative 모델보다 더 성능이 우수하다

10. model accuracy와 model performance 중 무엇이더 중요할까?
- model accuracy는 오로지 model performance 중에 하나다.

11. F1 score 가 무엇이고 어떻게 사용해야 하는 것인가?
- https://blog.naver.com/pertisia/222317648494

12. imbalanced dataset은 어떻게 다룰까?
- imbalanced 하더라도 일단 더 많은 데이터를 구해보자
- 데이터를 알맞게 resample 하기
- 이 데이터셋에 맞는 다른 알고리즘을 시도해보기
- 그 외에도 몇가지 tactics가 더 있음 (자세한건 프린트 링크 참고)

13. 언제 regression이 아닌 classification을 사용해야 할까?
