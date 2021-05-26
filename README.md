# 🐨코알라의 Kaggle 도전일지🦜

## Dogs vs Cats
https://www.kaggle.com/c/dogs-vs-cats

### #01.Keras CNN Classification
#### Ver.01 (0.9171)
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
- val_loss: 0.2044 , **val_accuracy: 0.9171** , epoch : 36/50 
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

