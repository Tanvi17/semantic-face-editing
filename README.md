DiscoGAN
=========================================

Prerequisites
-------------
   - Python 3.8
   - PyTorch
   - Numpy/Scipy/Pandas
   - Progressbar
   - OpenCV


Training DiscoGAN
----------------

Download CelebA dataset using:

    $ python ./datasets/download.py celebA 

(Currently, the link for downloading [CelebA](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) dataset is not available).

To train gender conversion:

    $ python ./discogan/image_translation.py --task_name='celebA' --style_A='Male'

To train hair color conversion:

    $ python ./discogan/image_translation.py --task_name='celebA' --style_A='Blond_Hair' --style_B='Black_Hair' --constraint='Male'


Results
----------------

Example result shows x_A, x_AB, x_ABA and x_B, x_BA, x_BAB

To check hair color conversion, visit

<img src="assets/b2b.png" width="600px">


Gratitude
----------------
This project would not be possible without the mentorship of Prof. J. Kao and TAs of course ECE 247: Neural Networks and Deep Learning.
A huge shoutout to SKT-Brain for DiscoGAN. Checkout the reference here: https://github.com/SKTBrain/DiscoGAN

