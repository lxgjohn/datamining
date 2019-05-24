# datamining

## 数据探索和分析
1. 重复值分析： 查看data.duplicated() ，删除重复值 data.drop_duplicates()；
2. 类型转换：分类值使用labelcode编码，文本转换成数值等；
3. 日期格式转换：pd.to_datetime()；
4. 缺失值处理：查看data.isnull()，空值填充data.fillna()；
5. 数据切分：使用sklearn.model_selection中train_test_split类

## 特征工程
1. 随机森林进行特征选择：使用sklearn.ensemble中RandomForestClassifier类，重要特征使用forest.feature_importances_获取

## 模型构建（fit-predict）
1. 逻辑回归：sklearn.linear_model中LogisticRegression
2. SVM：sklearn.svm中SVC
3. 决策树：sklearn.tree中DecisionTreeClassifier
4. 随机森林：sklearn.ensemble中RandomForestClassifier
5. XGBoost：使用xgboost中XGBClassifier

## 模型评价
1. 分类指标：使用sklearn.metics中classification_report， 展示结果 classification_report(预测值，真实值)
2. auc值：使用sklearn.metics中accuracy_score， 展示结果 accuracy_score(预测值，真实值）
3. roc_curve：使用sklearn.metics中roc_curve， 展示结果 roc_curve(真实值，预测值）

## 模型优化
1. 网格搜索法：使用sklearn.model_selection中GridSearchCV，查看最佳参数gridsearch.best_params_

## 模型融合
1. stacking融合：使用mlxtend.classifier中StackingClassifier
