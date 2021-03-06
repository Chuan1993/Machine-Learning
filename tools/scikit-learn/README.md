# scikit-learn
### 常用
* 划分验证集

```python
from sklearn.cross_validation import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=0)
```
* Grid Search 
```python
param_grid = {'n_estimators': [300, 500], 'max_features': [10, 12, 14]}
model = grid_search.GridSearchCV(estimator=rfr, param_grid=param_grid, n_jobs=1, cv=10, verbose=20, scoring=RMSE)
model.fit(X_train, y_train)
```


### 实现
* [常用算法调用(LR/RF/GBDT/knn)](./useful.py)
* [logistic回归](./sklearn_LR.py)

### Choosing the right estimator

![Choosing the right estimator](./choose.png)






