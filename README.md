# Engineering-Accomplishments

At the end of the interview Wednesday, Iman asked me to list my three most meaningful engineering accomplishments. I was able to list three projects I was proud of, however, I wanted to provide metrics to accurately demonstrate my ability to engineer and problem solve. It is apparent to me that this team is world-class. From providing power to Ukraine and Puerto Rico in times of need to reducing the world's reliance on fossil fuels, this team is changing the world. I want in. I have what it takes to excel, not just in this role, but on this team and at Tesla as a whole. I will stop at nothing to provide maximum value for all stakeholders. 

Below are my short bullet-point summaries of my top three engineering accomplishments. Below those are explanations of why the accomplishments are meaningful. Feel free to contact me with any questions or suggested edits. 

Bullet points: 

<ol>
  <li>
Collect a dataset and increase labeling throughput 5 fold while maintaining human-level accuracy by using unsupervised clustering methods. Created an image vectorization framework and evaluated different clustering models. To solve this problem in a time-constrained manner I needed to distribute computing across multiple cloud nodes. 
  </li>
  <li>
Create an object detection system that scans a room for items that the end-user inputs into the system. Five images of each item are collected and a novel few-shot learning method is used to train a model to locate the items. Was able to find items with over a 99.5% success rate on demo day. My team and I effectively worked together over two semesters. 
  </li>
  <li>
Create a custom convolutional layer that takes advantage of sparsity by having an irregular non-rectangular kernel shape. I effectively acted as a leader in a graduate student setting. ResNet50 accuracy on Cifar-10 was increased by 1.9 percent on the test set when compared to the control model with normal convolutions. 
  </li>
 </ol>
Explanations:
<ol>
  <li>
To learn about dealing with larger data, I decided to collect my dataset. Labeling was needlessly slow so I automated the process using unsupervised methods. Initially, I created a ‘proof of concept’ and debugged my method using the MNIST dataset. This allowed me to quickly iterate on simple data so I could develop a robust system faster. In order to create a vectorization model, I modified a classification CNN and used NCE loss, which is more often used in NLP. I implemented the loss function efficiently while maintaining readability. I decided to use TANH as my output layer activation function since, unlike sigmoid and relu, it is symmetric around zero making it a good candidate for vectorization. Once the MNIST prototype was functional I switched to developing on my dataset. Since I was crunched for time I had to scale my vectorization CNN hyperparameter searches over multiple GPUs in the cloud. Additionally, I needed to evaluate a choice of a clustering algorithm. I conducted a series of sweeps and random searches to tune the hyperparameters of DBSCAN and KMeans. I learned about the hyperparameters and inner workings of both algorithms but specifically DBSCAN. This engineering accomplishment shows my ability to solve complex problems under time constraint in an efficient way using a broad range of tools.
  </li>
  <li>
My capstone project is an end-to-end automated system that can identify an item in a messy room. I worked with a team for two semesters. My team did not organize their code in the same way I did so I learned to effectively work with people who think and organize in unique ways. Users are not going to collect and label hundreds or thousands of images of each item with bounding box labels, so we automated the process by creating an artificial dataset using a custom few-shot learning approach. Often I had to step outside of my comfort zone. For example, I took up the task of designing and 3D printing a prototype gimbal to hold the camera even though I had little experience with mechanical systems. This project has demonstrated my ability to think creatively and go outside of my comfort zone to solve problems. Additionally, working with my team for two semesters shows my ability to effectively collaborate with team members over an extended time. 
  </li>
  <li>
After reading a paper that took advantage of irregular-shaped convolutional kernels to speed up inference, I realized that a similar method could probably be used to increase accuracy during training. The idea is to use randomly shaped kernels rather than regularly shaped rectangular convolutional kernels. This takes advantage of kernel sparsity; since the kernels have different shapes they are forced to learn different features. I acted as the team lead even though I was an undergraduate and my teammates were graduate students. I delegated the PyTorch implementation to one team member, the Keras implementation to myself, and the third team member was in charge of research and testing. I organized bi-weekly meetings with the team where we checked in on our Gantt chart and talked about weekly progress and thoughts going forward. Since the team had other classes and responsibilities I would check in with my teammates to make sure their workload was manageable. The implementation was not specific to one framework, so I abstracted the problem in a framework-agnostic way. To complete this project I needed to learn how Keras and TensorFlow are structured. I demonstrated my ability to take a leadership role in a complex project and the ability to conceptualize and implement state-of-the-art ideas. 
</li>
</ol>
