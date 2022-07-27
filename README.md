# Increase-your-RAM-in-Google-colab
some of you may have trouble while working on Google colab. For free users, colab only gives 12GB ram, for some large model, it will result in crashdown. here is the website that could increase your RAM to 25GB.  

https://colab.research.google.com/drive/155S_bb3viIoL0wAwkIyr1r8XQu4ARwA9  

Open that notebook and save it as a copy in your colab notebook, open that copy and connect it, then you will get a 25GB RAM notebook.    

If you want to use GPU to train your model, here is the code to check whether GPU is successfully deployed on your colab:  

!nvidia-smi -L 

If you want to use the data in colab, you may need to upload it into colab from your computer, for some large data, it might be inconvenient. 
A easier way is to upload your data to your Google drive first then call them from Drive, you can just run this code:  

import os from google.colab import drive drive.mount('/content/drive')
