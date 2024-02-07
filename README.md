# AlexNetTransferLearning

AlexNet was Fine Tuned to a binary classification task (Chair or Wine bottle) 

* Pretrained AlexNet model was first loaded using __torchvision__.

* Uploaded the images I am interested in classifying (Chair/Wine bottle).

* Randomly Augmented these images to increase sample size and variation (__PIL__).

* Created Custom __Dataset__ and __DataLoader__.

* All the layers in AlexNet were frozen (requires_grad=False).

* The last Linear Layer was replaced with a Sequential Layer (Linear and ReLU) with a drop out of .4.

* This was fed to a sigmoid for my binary classification (Chair or Wine bottle)

* Trained and Validated my model
