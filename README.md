**Custom-Resent model**

**Introduction**

The goal of this project is impelement custome resenet model on the CIFAR10 datset using pytorch.this projects demonstrates how to develop Resnet architecture,data agumentation statergies, custom dataset classes, and learning rate schedulers.

**Methodology**

 The project is organized as follows: 
 
 1.Data Loading and Preprocessing

 2.Dataset statistics calcualtion

 3.Data Agumentation statergy 

 4.Development of Model
 
 5.Performance of the Developed model

 **Data Loading and Preprocessing**

 In the fields of machine learning and computer vision, the CIFAR-10 dataset is considered a benchmark dataset due to its widespread use.CIFAR-10 is utilised in a large number of research publications and projects in order to evaluate and compare the performance of various machine learning algorithms and neural network designs.It is a widely used dataset for research into novel computer vision techniques as well as their development.If you would like to learn more about cfar10, please click the link below.

  https://www.cs.toronto.edu/~kriz/cifar.html

On the train dataset, we applied the normalisation, padding, random cutting, and horizontal flipping data argumentation strategies.These mentioned strategies are implemented from the albumentations library.

 **Data Agumentation statergy**
 
 ![image](https://github.com/kiran-pyt/Custom-Resnet/assets/120393460/32351e32-df4a-46c9-a520-c3a091af8c96)

  **Images After Applying Data Agumentation Statergy**

 ![image](https://github.com/kiran-pyt/Custom-Resnet/assets/120393460/53654f63-b443-449d-92d9-6371b9f0b597)

 **Development of Model**

 ![image](https://github.com/kiran-pyt/Custom-Resnet/assets/120393460/43564cfc-8895-4e6d-b9f0-afe12cb14a29)

 **Performance of the Developed model**

 ![image](https://github.com/kiran-pyt/Custom-Resnet/assets/120393460/2b567532-2812-4068-92d0-97cb948841be)



 The "One Cycle Policy" is a technique used in training deep learning neural networks, particularly in the context of training convolutional neural networks (CNNs) and neural networks for tasks like image classification. It was introduced by Leslie N. Smith in a paper titled "Cyclical Learning Rates for Training Neural Networks." The One Cycle Policy is designed to help find an optimal learning rate schedule for training neural networks, improving training speed and convergence.

Here's all you need to know about the One Cycle Policy:

1. **Learning Rate Schedule**:
   - The One Cycle Policy involves cycling the learning rate during training by gradually increasing it from a small value to a maximum value and then decreasing it back to a small value.
   - Typically, this cycle spans over a few epochs during training.

2. **Key Components**:
   - There are two key components to the One Cycle Policy:
     - **Learning Rate Range**: The learning rate starts at a small value (e.g., 1e-5) and gradually increases to a maximum value (e.g., 1e-2) during the first half of the cycle. Then, it decreases back to the initial small value during the second half.
     - **Momentum Schedule**: In addition to changing the learning rate, the policy also adjusts the momentum (a hyperparameter that controls the update step size during optimization) inversely. As the learning rate increases, momentum decreases, and vice versa.

3. **Benefits**:
   - The One Cycle Policy has several benefits:
     - Faster convergence: It often leads to faster convergence and can reduce the number of training epochs required to achieve good results.
     - Better generalization: It can improve the model's ability to generalize to new data by exploring a broader range of learning rates.
     - Regularization effect: The cyclical learning rate and momentum schedules can act as a form of regularization, helping to prevent overfitting.

4. **Implementation**:
   - Implementing the One Cycle Policy requires adjusting the learning rate and momentum during training according to the specified schedules.
   - Most deep learning frameworks and libraries, such as PyTorch and TensorFlow, provide built-in support for implementing the One Cycle Policy.

5. **Finding the Right Parameters**:
   - The specific values for the minimum and maximum learning rates, as well as the duration of the cycle, may need to be tuned for each specific task and architecture.
   - Hyperparameter tuning techniques like grid search or random search can be used to find optimal values.

6. **Applications**:
   - The One Cycle Policy can be applied to various deep learning tasks, including image classification, object detection, and natural language processing.
   - It has been widely adopted in the deep learning community and is often used in conjunction with techniques like the "learning rate finder" to determine appropriate learning rate ranges.

In summary, the One Cycle Policy is a learning rate scheduling technique that helps accelerate the training of neural networks, improve convergence, and enhance generalization. It has become a valuable tool for practitioners in the field of deep learning and is often used in combination with other training strategies to train more effective models.

![image](https://github.com/kiran-pyt/Custom-Resnet/assets/120393460/a4388a83-f3d9-4c34-bb4b-0c0283e207d4)

please click the link below to know more about one cycle policy.

https://medium.com/dsnet/the-1-cycle-policy-an-experiment-that-vanished-the-struggle-in-training-neural-nets-184417de23b9




 



            

          










 





