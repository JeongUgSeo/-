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
- 카테고리로 나누어지는 결과를 얻길 원할때 classification을 사용하면 된다

14. 앙상블 테크닉을 쓰기 좋은 예시를 열거해보아라
- 앙상블 기술은 learning algoright들을 결합해서 사용한다. 그렇게 해서 좀더 좋은 퍼포먼스를 최적화 한다.
- 오버피팅을 줄어주며 모델이 보다 robust해진다. (training의 작은 변화에도 크게 영향을 받지 않는다)
- 앙상블의 예시로는 bagging, boosting, the 'bucket of modesl' method) 등이 있다.

15. 오버피팅 하지 않는 다는것을 어떻게 확신할 수 있는가?
- 3가지의 주요한 방법이 있는데
- 모델을 좀더 simple하게 만드는 것이다. 매우 작은 숫자의 변수와 파라미터가 되도록 분산값을 감소시킨다. 그러면 training data의 noise를 감소시킬 수 있을 것이다.
- k-folds cross-validation과 같은 cross-validation 기법들을 사용하는 것이다.
- LASSO와 같은 regularization 기법들을 사용함으로서 모델 파라미터를 오버피팅이 되지 않도록 penalize 하는 것이다.

16. 어떤 평가 방법이 머신러닝 모델의 효과를 입증하는데 유용할것이냐?
- F1 score, accuracy, confusion matrix 중에서 선택을 하면 되는데
- 아래에 각각에 대해서 잘 정리되어 있는 list가 있고
- https://machinelearningmastery.com/classification-accuracy-is-not-enough-more-performance-measures-you-can-use/
- 아래에는 좀더 읽을 만한 내용이 있음
- https://machinelearningmastery.com/how-to-evaluate-machine-learning-algorithms/
- (한글사이트)
- https://blog.naver.com/owl6615/222030981012
- https://blog.naver.com/whdals0/222305204768
