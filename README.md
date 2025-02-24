# Practical-DL-Assignments
- Assignment 1 - Revisiting basic of ML and DL
## Assignment 2 
### Training and I/O Optimization: 
We analyzed the impact of data loader worker count on training efficiency for a ResNet-18 model on CIFAR-10 using PyTorch. By sweeping worker counts at different step sizes, we observed variations in optimal values. We developed an adaptive worker allocation strategy based on system metrics like CPU/GPU utilization. This approach aims to improve training speed by dynamically adjusting the number of workers.

✅Findings:

A coarse-grained sweep (step of 4) suggested an optimal worker count of 4, while a fine-grained sweep (step of 1) found 2 to be better. This highlights that worker optimization requires finer tuning for best efficiency. 🚀

### Seq2Seq Chatbot - Model Deployment, Serve and Batch Prediction
We developed a Seq2Seq chatbot using PyTorch for conversational AI.
We optimized model performance with Wandb, conducting a sweep search over various hyperparameters.
The chatbot was deployed via a Flask API for real-time interactions. 
To ensure scalability, we used Ray for efficient, distributed batch inference.

✅ Result: 

A production-ready, high-performance chatbot with optimized responsiveness. 🚀
