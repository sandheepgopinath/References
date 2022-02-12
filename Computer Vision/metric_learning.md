# Metric Learning and Siamese Network

- Traditional Image processing methods needs large number of images
- orFr face recognition, if we use a taditional classification using CNN the image will have to be trained with large number of samples. And it required retrainining with large samples to effectively detect the person
- Periodic retraining is costly


##### One Shot Learning 
![](https://miro.medium.com/max/960/1*g-561DsAfbU6gcVEk9AC4g.jpeg)
- The idea begind this architecture is to use a reference image and find the similarity with the image to be tested
- Siamese network helps in finding the similarity

## Concept of Metric Learning
Metric is like a distance. 
Properties of distances
- Always positive
- Follows triangle inequality. 
![](https://www.onlinemathlearning.com/image-files/triangle-inequality.png)
- Inverse of similarity. Smaller the distance, larger the similarity
Symetric : distance between a-b = distance between b-a
- Metric learning is the task of leanring a distance function over objects

Eg : Eucledian distance, Mahnattan distance etv

## Siamese network
![](https://miro.medium.com/max/1400/1*LwOBbwGXMZUy6OzkFAPTzw.png)

- Reference image is converted into embedding.
- So is the test image
- The embedding can be generated by any networks like Lenet, AlexNet etc
- The embeddings are then compared to see how similar the two metrics are