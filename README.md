
# END_3_0_Assignment_Session_1

Assignment for Session 1 - Background & Very Basics (END3.0)


**1)	What is a neural network neuron?**

- It’s a building block of a neural network which stores a value temporarily.

**2)	What is the use of the learning rate?**

![s1](https://user-images.githubusercontent.com/56379895/134590343-11b601a3-0a5c-45f0-8381-4da46832e114.jpg)

- Let’s assume we are calculating the new weight update for w2, In this scenario the confusion will be that whether we should consider the old w1 value or the new updated weight w1 if w1 is influencing w2. And if we keep considering the new updated values every time when we compute new values for subsequent weights we will be stuck in an infinite loop. 

![s2](https://user-images.githubusercontent.com/56379895/134590474-9ffc0402-3db6-4f42-9b55-b1d31e0a9ab7.jpg)

- Hence to resolve this issue partial derivatives comes in to picture, where we will assume that while computing update for a specific weight, all the other weights remain constant. And while doing so before updating any weight we multiply the partial derivatives (gradients) with a smaller value called Learning Rate (LR) because even if there was some kind of impact from w1 on w2, this LR will make the updates so small that the influence of w1 on w2 will become mathematically insignificant.

**3)	How are weights initialized?**
- Generally weights are initialized randomly between 0 & 1 Because initializing all the weights to same value or to 0.0 will result in some kind of asymmetry in the error gradient which will begin searching in effectively. And mostly the weights are normalized to be under one scale and mostly be nearest to zero because this will make sure that the feedback from backpropagation will make sense for all the values computed in the hidden layers while computing gradients.

**4)	What is "loss" in a neural network?**
- Loss is the difference between the predicted and the actual output value. 

**5)	What is the "chain rule" in gradient flow?**
- Chain Rule is something which enables the backpropagation to happen effectivity by considering the contribution from the other neurons. 
![s3](https://user-images.githubusercontent.com/56379895/134590501-30e98785-07cc-4362-a312-e13b003e5202.jpg)

  
