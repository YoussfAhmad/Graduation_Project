# CNN First run:
the first run of the cnn we tryed to run the augmente the data to 12k per class and take the validation data from train copy 
Epoch 40/40
2930/2930 - 994s - loss: 0.3767 - acc: 0.8631 - val_loss: 0.7517 - val_acc: 0.8140 - 994s/epoch - 339ms/step
219/219 [==============================] - 21s 94ms/step - loss: 0.7817 - acc: 0.8058
Test accuracy: 0.8058099746704102
# CNN Second run:
we droped the  half  of largest calass ("NV" to aprrox. 6k) and augmented the data to 6k train and validation to 1300
Epoch 45/45
1422/1422 - 483s - loss: 0.1802 - acc: 0.9371 - val_loss: 4.1895 - val_acc: 0.4539 - 483s/epoch - 339ms/step
160/160 [==============================] - 18s 115ms/step - loss: 4.3153 - acc: 0.4526
Test accuracy: 0.4525718688964844
# CNN third run:
 droped the  half  of largest calass ("NV" to aprrox. 6k) and Shuffle and augmented the data to 6k train and validation to 1300
Epoch 45/45
1394/1394 - 484s - loss: 0.3121 - acc: 0.8868 - val_loss: 3.5633 - val_acc: 0.4440 - 484s/epoch - 347ms/step
155/155 [==============================] - 14s 92ms/step - loss: 3.6100 - acc: 0.4407
Test accuracy: 0.4406950771808624
# CNN fourth run:
Data shuffled and droped the  half  of largest calass only augmented the smallest 4 classes to 6k 
Epoch 45/45
1093/1093 - 330s - loss: 0.1530 - acc: 0.9471 - val_loss: 3.4167 - val_acc: 0.5530 - 330s/epoch - 302ms/step
126/126 [==============================] - 10s 79ms/step - loss: 3.2714 - acc: 0.5609
Test accuracy: 0.5608847141265869
# CNN fifth run:
data shuffled and augmented only the smallest 4 classes to 5k
# New CNN Architecture :
Data shuffled and droped the  half  of largest calass only augmented the smallest 4 classes to 6k 
Train: 82 Val: 64 Test: 63.3
# VGG_Trial_3
This trial's structure is the VGG Architecture which consists of 2 Conv2D layers then a Max Pooling layer
No Pre Processing but the data is augmented up to 5000 image per class in train and 1000 for validation
input size=32*32
( Train:80,test:20)
accuracy=63%
# VGG_Trial_4
This trial's structure is the VGG Architecture which consists of 2 Conv2D layers then a Max Pooling layer
No Pre Processing or data augmentation was done , input size =32*32,
( Train:80,val:10,test:10)
accuracy=64%
