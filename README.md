# Final
## Support Vector Machines

주어진 데이터를 판단하기 위해 svm 모델을 사용하였다.

    X_train, X_test, y_train, y_test = sklearn.model_selection.train_test_split(X, y, test_size=0.0001, random_state=0)

먼저 주어진 데이터를 이용하여 train 할시 정확도를 최대한 높이기 위해 test_size 를 최소화 하여 train 에만 집중하였다.

    clf = SVC(C=5, kernel="rbf",gamma = 11, random_state=100)

다음으로 svm 모델을 설정하는 과정에서 kenal 은 기본형 RBF를 이용하였고 이에따라 조정해야할 parameter 를 조정해주었다. 조정할 C 값과 gamma 값에 대해 C는 기본값인 1 보다 오류를 덜 허용하기 위해 5로 설정하였고 gamaa 값은 25로 하였을때 오버피팅이 일어나 정확도가 떨어지는 것 같아 11로 설정하였다.

    
