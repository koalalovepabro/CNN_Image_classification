# 🐨코알라의 Kaggle 도전일지🦜

## [Dogs vs Cats](https://www.kaggle.com/c/dogs-vs-cats)
---
### #01. [Keras CNN Classification](https://www.kaggle.com/uysimty/keras-cnn-dog-or-cat-classification)
### Ver.01 (0.9171)
- val_loss: 0.2044 , **val_accuracy: 0.9171** , epoch : 36/50 
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
- val_loss: 0.4513 , **val_accuracy: 0.7952** , epoch : 6/50
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
- val_loss: 0.2044 , **val_accuracy: 0.9143** , epoch : 38/50 
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
 ---
### #02. [Feature extractor fine tuning with Keras](https://www.kaggle.com/angqx95/feature-extractor-fine-tuning-with-keras)
### Ver.01 (0.9844)
- val_loss: 0.0345 , **val_accuracy: 0.9844** , epoch : 5
- Run on Kaggle ( GPU )
- MGD(Mini-Batch Gradient Descent)
- Feature Extractor : VGG16 + Logistic Regression
- Fine Tuning : ResNet50
- compare "Custom CNN / Transfer Leearn(VGG16) / Fine Tune(ResNet)

---
### #03. [Vanila CNN & ResNet50](https://www.kaggle.com/bhuvanchennoju/hey-siri-is-it-a-or-f1-0-992/output)
### Ver.01
