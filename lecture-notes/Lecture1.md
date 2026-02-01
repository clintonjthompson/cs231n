## Lecture 1
YouTube link [here](https://www.youtube.com/watch?v=2fq9wYslV0A&list=PLoROMvodv4rOmsNzYBMe0gJY2XS8AQg16&index=1)

1. Computer Vision is embedded in Artificial Intelligence and overlaps with (statistical) machine learning. Deep learning is captured in machine learning. Thus this course is the intersection of deep learning and computer vision. 
2. Brief history of CV and deep learning:
   1. Crux of course is how visual intelligence happens.
   2. Research in late 1950s using cats showed that neurons in visual cortext of brain process specific parts of images, e.g. vertical lines, with each neuron focusing on limited area. Also found that visual pathway is hierarchical. As move up hierarchy, gets more complex. For example, process vertical lines first, then corners, then objects. 
   3. Early and late 1960s saw first academic work (ph.d. dissertation) and a summer project to "solve" computer vision. Needless to say, CV was not solved. 
   4. 1970s saw research in trying to infer full dimensionality of objects (3D) based on 2D processing. This is an inherently hard problem that vexes CV to this day. 
   5. 1980s: Work in recognition via edge detection following emergence of digital photos.  
   6. AI winter arrives but research continues (1980s-1990s).
> "Visual recognition is a fundamental task for visual intelligence."
   7. Face recognition in early 2000s. 
   8. Mid-aughts: convergence of digital images and internet led to availability of data. 
   9. 1986: Big breakthrough with "backpropagation" (Rumelhart, Hinton, & Williams, 1986). Compute gradients in neural networks. An error correction function. Propagate error back to input using basic calculus chain rules. 
   10. 1998: LeCun, et al when working at Bell Labs. Convolutional Networks: applied backprop algorithm to a Neocognitron-like architecture that learned to recognize hand-written digits. Very similar to modern CNNs. 
   11. 2000s: "Deep Learning". Lack of data make it difficult to train and improve models. Data required to let models learn to generalize. 
   12. Late 2000s let to creation of ImageNet (Large Scale Visual Recognition Challenge) to shore up lack of data. 1,000 object classes; 1.4 images. 
       1.  Error rates abysmal until 2012 when AlexNet (Hinton, et al.) used deep learning (and backpropagation) to reduce error rate significantly. Backpropagation reduce reliance on building network by hand (NeoCognitron) and was mathematically rigorous. Availability of data also key. This mark the historical moment of rebirth of deep learning revolution. 
   13. 2012 - Present: Deep learning is everywhere. Image classification, image retrieval, object detection, image segmentation, video classification, activity recognition, pose recognition, medical imaging, galaxy classification, image captioning, relationships of objects in images, generative AI (DALL-E)
   14. Three converging forces -- computation, algorithms, data -- lead to current innovation and practice of CV. 
3.  CV has a long way to go. Problem is not solved. Biases remain an issue because data reflects human biases. 
4.  Course Overview:
    1.  What is CV? Enabling machines to see and understand images. Most fundamental task is image classification. This task is foundation for more complicated tasks. 
    2.  How teach machine to do this? Linear classification is one way to do this. Limited power. Not work well data not clearly delineated. Regularization and optimizaton can be used to improve models and allow generatlization.
    3.  Neural Networks: unlike linear models, they stack multiple layers to model non-linear functions. These models pretty much power all modern tools and capabilities. 
    4.  Perceiving and Understanding the world: Tasks at hand rely on different models. Create systems that can "see" and interpret the world around us. 
        1.  Tasks beyond classification: classification - no spatial extent --> semantic segmentation (grass, cat, sky, tree) - no objects, just pixels --> object detection (dog, cat) --> instance segmentation (dog, cat)
        2.  Beyond Multi-Layer Perceptron: Convolutional Neural Networks (CNN). Also learn recurrent neural networks for sequential data. 
    5.  Generative and Interactive Visual Intelligence
        1.  Self-supervised learning. Training models that don't require pre-labeled data. 
        2.  Generative modeling: DALL-E, DALL-E 2, Diffusion Models, 
        3.  Vision Language Models: Connect text and images in a shared representation space. Given caption, model generates the image. 
    6.  Human-Centered Applications and Implications  

