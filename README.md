My first major machine learnign project, after some other small projects like a number recognizer, cat/dog classifier, etc. 
In this project I designed a custom model in an attempt to remove watermarks from images, and the results were so-so. 
There already exist versions of this that do much better, but I was looking to do some sort of image to image machine learning project and the idea came to mind. 
The model follows a variational autoencoder architecture, which I did with PyTorch.
I trained off of an existing dataset of 60,000 images of watermarked and their non watermarked equivalent images. 

In the end, I had lots of compression artifacts, but the image was roughly recreated. As a result of it being blurry, I guess the watermark was slightly less noticeable? 
I ended up basically creating a not-great compresssion algorithm. If I were to do this again, I would likely try to recreate the U-net architecture, which I think would improve model performance drastically.

If you run "Cole_westerveld-Running_The_Model.ipynb" and you uncomment the first bit of code to download the dataset it will randomly pick a picture to run the model on
It takes ~5mins to download dataset.
Also may need img.show() to dfisplay images, but that doesnt work on google colab so just keep as display(img) if using on colab

To all the photographers I SWEAR im not evil or would use this for anything bad...
theres other already good tools that could do the same thing but 10x better
just a fun idea for my first serious ML project

