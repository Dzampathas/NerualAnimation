##### Disclaimer 

Because Neural Networks create very large files, it's a little difficult to upload everything to this repository. For now I'll have to only upload results and training data.

## In this project 
I primarily used pix2pix tensorflow https://github.com/affinelayer/pix2pix-tensorflow to train a Neural Network on my sketches and polished drawings to see if it could render an animation solely from sketches alone.

## Initially
 I tried to train the network on as little as I possibly could, which didn't result in anything very astounding... What appeared was almost demonic..
 It was a good start though, I needed to give it more training data, and that's where I went.
 
## Eventually
  I wound up training the network on all the cleaned up drawings for the animation, and it created something fairly reasonable, relatively polished. Though, I am not sure if it could reproduce that for a foreign set of drawings.
  If the network was given a massive training set to work off of, the pix2pix algorithm could most definitely be used to clean up animation. But I don't think it is worthwhile. To produce anything good enough would require more time and effort than it would to produce the clean drawings yourself.
  
## Conclusion
  Pix2pix is only one part of the picture for creating a neural network that could properly render 2D animation. Either having an optimal training set that exposes the network to every needed outcome, or creating a smarter algorithm that can identify parts of the sketch and generate images based on smaller but more intelligent information. 

https://drive.google.com/open?id=1ea4RicU_uz0pfvFU8IBUbNEUrvBBU5Qj

#### Training code

> python pix2pix.py \
  --mode train \
  --output_dir al_train1 \
  --max_epochs 300 \
  --input_dir al_Anim1/ \
  --which_direction AtoB
  
 
