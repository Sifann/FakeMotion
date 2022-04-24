# IJCAI-2022-FakeMotion
One compelling application of artificial intelligence is to generate a video of a target person performing arbitrary desired motion (from a source person). While the state-of-the-art methods are able to synthesize a video demonstrating similar broad stroke motion details, they are generally lacking in texture details. A pertinent manifestation appears as distorted face, feet, and hands, and such flaws are very sensitively perceived by human observers. Furthermore, current methods typically employ GANs with a L2 loss to assess the authenticity of the generated videos, inherently requiring a large amount of training samples to learn the texture details for adequate video generation. In this work, we tackle these challenges from three aspects: 1) We disentangle each video frame into foreground (the person) and background, focusing on generating the foreground to reduce the underlying dimension of the network output. 2) We propose a theoretically motivated Gromov-Wasserstein loss that facilitates learning the mapping from a pose to a foreground image. 3) To enhance texture details, we encode facial features with geometric guidance and employ local GANs to refine the face, feet, and hands. Extensive experiments show that our method is able to generate realistic target person videos, faithfully copying complex motions from a source person. 
![image](https://github.com/Sifann/FakeMotion/main/method.png)
