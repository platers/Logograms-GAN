
Recently I watched the movie Arrival(about an alien language)  and did some reading about the language used in the film. 

The symbols (called logograms) are very elegant:

<img src="/logos/Heptapod1.jpg" width="200"/><img src="/logos/IanLouiseMustGo1.jpg" width="200"/><img src="/logos/MustLearnIanLouise1.jpg" width="200"/>

The creators uploaded some of the symbols to github for public use. I used these 40 logograms and trained a GAN on them. I coded the GAN(DCGAN to be precise) in keras (with a lot of help from other projects on github) and modified it a bit to work for logograms. In the end I was able to generate 128x128 pixel images:

<img src="/examples/dirty.png" width="200"/><img src="/examples/dirty1.png" width="200"/><img src="/examples/dirty2.png" width="200"/>

These images are certainly not as clean as the originals but they are unmistakably similar. I wrote a simple script to clean up these images by removing stray marks.

<img src="/examples/clean.png" width="200"/><img src="/examples/clean1.png" width="200"/><img src="/examples/clean2.png" width="200"/>

Unfortunately these images look like copies of the original logograms. I believe this is because of the small number of samples. Hopefully the producers will release more of the language in the future. Some future work I hope to do is to use CPPN's to produce images of much higher resolution.