# 🐨코알라의 Kaggle 도전일지🦜

## [Dogs vs Cats](https://www.kaggle.com/c/dogs-vs-cats)
---
### #01. [Keras CNN Classification](https://www.kaggle.com/uysimty/keras-cnn-dog-or-cat-classification)
### Ver.01 (0.9171)
- val_loss: 0.2044 , **val_accuracy: 0.9171** @epoch 26, epochs : 36/50 
- Keras CNN Classification
- Run on Colab
- `earlystop = EarlyStopping(monitor='val_loss', patience=10)`
- `learning_rate_reduction = ReduceLROnPlateau  
(monitor='val_accuracy',  
                                           patience=2,  
                                           verbose=1,  
                                           factor=0.5,  
                                           min_lr=0.00001  
                                           )` 
                                           
### Ver.02 (0.7952)
- val_loss: 0.5258 , **val_accuracy: 0.7952** @epoch 4, epochs : 6/50
- Keras CNN Classification
- Run on Colab

- **학습조기종료, 학습률 자동감소 조건 변경**
- `earlystop = EarlyStopping(monitor='val_accuracy', patience=2)`
- `learning_rate_reduction = ReduceLROnPlateau  
(monitor='val_loss',  
                                           patience=10,  
                                           verbose=1,  
                                           factor=0.5,  
                                           min_lr=0.00001  
                                           )`
                                           
### Ver.03 (0.9143)
- val_loss: 0.2238 , **val_accuracy: 0.9143** @epoch 32, epochs : 38/50 
- Keras CNN Classification
- **Run on Kaggle ( GPU )**

- `earlystop = EarlyStopping(monitor='val_loss', patience=10)`
- `learning_rate_reduction = ReduceLROnPlateau  
(monitor='val_accuracy',  
                                           patience=2,  
                                           verbose=1,  
                                           factor=0.5,  
                                           min_lr=0.00001  
                                           )` 
                                           
### Ver.04 (0.9189)
- val_loss: 0.2465, **val_accuracy: 0.9189** @epoch 37, epochs : 37/50
- Keras CNN Classification
- Run on Kaggle ( GPU )
- **batch_size를 5에서 128로 변경**
- `earlystop = EarlyStopping(monitor='val_loss', patience=10)`
- `learning_rate_reduction = ReduceLROnPlateau  
(monitor='val_accuracy',  
                                           patience=2,  
                                           verbose=1,  
                                           factor=0.5,  
                                           min_lr=0.00001  
                                           )`                          
                                           
### Ver.05 (0.)
- val_loss:  , **val_accuracy: 0.** @epoch , epochs : /50
- Keras CNN Classification
- Run on Colab

- **batch_size를 5에서 128로 변경**
- **학습조기종료, 학습률 자동감소 조건 변경**
- **(EarlyStopping과 ReduceLROnPlateau의 모니터 모두 val_accuracy)**
- `earlystop = EarlyStopping(monitor='val_accuracy', patience=10)`
- `learning_rate_reduction = ReduceLROnPlateau  
(monitor='val_accuracy',  
                                           patience=5,  
                                           verbose=1,  
                                           factor=0.5,  
                                           min_lr=0.00001  
                                           )`
---
### #02. [Keras CNN, Transfer Learnings](https://www.kaggle.com/serkanpeldek/keras-cnn-transfer-learnings-on-cats-dogs-dataset)
### Ver.01 (0.9468)
- **val_accuracy: 0.9468**
- Run on Kaggle ( GPU )
- Feature Extractor : VGG16 + LogisticRegression
- Fine Tuning : None
- `cv_scores=cross_val_score(LogisticRegression(solver="lbfgs"), features, targets, cv=3 )`

---
### #03. [Feature extractor fine tuning with Keras](https://www.kaggle.com/angqx95/feature-extractor-fine-tuning-with-keras)
### Ver.01 (0.9844)
- val_loss: 0.0345 , **val_accuracy: 0.9844** @epoch 5, epochs : 5
- Run on Kaggle ( GPU )
- MGD(Mini-Batch Gradient Descent)
- Feature Extractor : VGG16 + Logistic Regression
- Fine Tuning : ResNet50
- compare "Custom CNN / Transfer Leearn(VGG16) / Fine Tune(ResNet)

---
### #04. [Vanila CNN & ResNet50](https://www.kaggle.com/bhuvanchennoju/hey-siri-is-it-a-or-f1-0-992/output)
### Ver.01 (0.982)
- **val_accuracy: 0.9892** @epoch 5, epochs : 5
- Run on Kaggle ( GPU )
- **Building model for transfer learning on top of pretrained ResNet50 Model**
