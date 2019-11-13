About kido:
-----------
Can we figure out what someone is typing, just by listening to the keystrokes?

This project called **kido** (= keystroke decode) explores if this is possible.
It is published in [Towards Data Science](https://towardsdatascience.com/clear-and-creepy-danger-of-machine-learning-hacking-passwords-a01a7d6076d5).


Quick start guide:
------------------
For training and validation: `kido/code/kido_train.ipynb`   
Training data at: `kido/images/train/`  
Validation data at: `kido/images/dev/`  
The training and validation images are stored as per TensorFlow convention.  
For example, all training images corresponding to keystroke `m` are stored in a subfolder `images/train/m`, 
and all validation images corresponding to keystroke `m` are stored in a subfolder `images/dev/m`, and so on.

For testing:  `kido/code/kido_test.ipynb`  
Specify the test dir, in this case: `kido/batch99_test/`  
In the test dir make four sub-dirs called `audio`, `images`, `model`, and `splits`  
Store the word-keystrokes m4a (unsplitted) at: `kido/batch99_test/audio/`  
Make sure the file name is the word itself (type only alphabets and all lowercase).  
For example `iloveu.m4a` should be the file name for the keystrokes audio typing `iloveu`.  
The python script will automatically convert m4a to wav, split, and generate spectrograms.  
Store the trained model at: `kido/batch99_test/model/` and specify the file name in the script.

Note: All the data (train, dev, and test) in this study were collected using my MacBook Pro (Retina, 13-inch, Early 2015) keyboard.


Detail descriptions:
--------------------
Coming soon ...


Resources:
----------
Published in Towards Data Science: https://towardsdatascience.com/clear-and-creepy-danger-of-machine-learning-hacking-passwords-a01a7d6076d5

The rockyou passwords link: https://www.kaggle.com/wjburns/common-password-list-rockyoutxt#rockyou.txt
