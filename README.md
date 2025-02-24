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

## Assignment 3
### SSD and ONYX
We fine-tuned the MobileNetV1 model for image classification and converted it to ONNX for cross-platform deployment. The model was optimized for faster inference using ONNX Runtime (ORT), ensuring quick and scalable predictions. 

✅ This solution enables efficient deployment on edge devices and cloud environments for real-time applications.

### Transfer Learning
We implemented transfer learning for image classification using a Convolutional Neural Network (CNN), exploring two approaches:
- Finetuning the ConvNet: We initialized the model with a pre-trained network (e.g., from Imagenet) and fine-tuned it on the target dataset.
- Base Model as Fixed Feature Extractor: We froze the pre-trained weights and only trained the final fully connected layer.
  
✅  Findings:
- Finetuned models outperformed fixed feature extractors, showing that fine-tuning all layers improves performance.
- Transfer learning provided significant performance gains with fewer training examples and reduced computational costs.
- Finetuning improved generalization, demonstrating the effectiveness of adapting pre-trained models to specific tasks.


