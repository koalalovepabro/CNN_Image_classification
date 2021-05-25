# 🐨코알라의 Kaggle 도전일지🦜
https://www.kaggle.com/c/dogs-vs-cats

## Ver.01 (0.9171)
- val_loss: 0.2044 , **val_accuracy: 0.9171** , epoch : 36/50 
- Keras CNN Classification
- `earlystop = EarlyStopping(monitor='val_loss', patience=10)`
- `learning_rate_reduction = ReduceLROnPlateau  
(monitor='val_accuracy',  
                                           patience=2,  
                                           verbose=1,  
                                           factor=0.5,  
                                           min_lr=0.00001  
                                           )` 
## Ver.02
EarlyStopping moniter = 
