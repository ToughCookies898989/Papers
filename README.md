# Intro
Combine CV with NLP tasks，place emphasis on Image/Video Captioning、Paragraph Description Generation and Medical Report Generation.
- [Image/Video Captioning](#image/video-captioning)
- [Paragraph Description Generation](#Paragraph-Description-Generation)

# Papers and Codes/Notes
### Image/Video Captioning
- CNN-RNN
	* Learning to Read Chest X-Rays- Recurrent Neural Cascade Model for Automated Image Annotation, CVPR 2016
	* TieNet Text-Image Embedding Network for Common Thorax Disease Classification and Reporting in Chest X-rays, CVPR 2018[(author's homepage)](https://xiaosongwang.github.io)
	* On the Automatic Generation of Medical Imaging Reports, ACL 2018, CMU[(author's homepage)](http://www.cs.cmu.edu/~pengtaox/)
	* Multimodal Recurrent Model with Attention for Automated Radiology Report Generation, MICCAI 2018, PSU
	* End-to-End Video Captioning with Multitask Reinforcement Learning
	* Move Forward and Tell- A Progressive Generator of Video Descriptions, ECCV 2018, CUHK

- CNN-CNN
	* Convolutional Image Captioning, CVPR 2018([code](https://github.com/aditya12agd5/convcap))

- Reinforcement Learning
	* Improving Reinforcement Learning Based Image Captioning with Natural Language Prior, 2018 

- Others
	* A Neural Compositional Paradigm for Image Captioning, NIPS 2018, CUHK

### Paragraph Description Generation


## 基本知识
* RNN
	* introduce of some blogs
		* [Written Memories: Understanding, Deriving and Extending the LSTM](https://r2rt.com/written-memories-understanding-deriving-and-extending-the-lstm.html), on this blog
		* [Recurrent Neural Networks Tutorial](http://www.wildml.com/2015/09/recurrent-neural-networks-tutorial-part-1-introduction-to-rnns/), by Denny Britz(I have read)
		* [The Unreasonable Effectiveness of Recurrent Neural Networks](https://karpathy.github.io/2015/05/21/rnn-effectiveness/), by Andrej Karpathy
		* [Understanding LSTM Networks](https://colah.github.io/posts/2015-08-Understanding-LSTMs/), by Christopher Olah
	* rnn in tensorfolw
		* [Recurrent Neural Networks in Tensorflow I](https://r2rt.com/recurrent-neural-networks-in-tensorflow-i.html)
		* [Recurrent Neural Networks in Tensorflow II](https://r2rt.com/recurrent-neural-networks-in-tensorflow-ii.html)
		* [Recurrent Neural Networks in Tensorflow III](https://r2rt.com/recurrent-neural-networks-in-tensorflow-iii-variable-length-sequences.html)

## 医学数据集(medical dataset)
* NIH Chest X-Ray([download link])(https://nihcc.app.box.com/v/ChestXray-NIHCC)
	* ChestX-ray8 Hospital-scale Chest X-ray Database and Benchmarks on Weakly-Supervised Classification and Localization of Common Thorax Diseases, CVPR 2017, NIH

## 经典任务
* 分类(classification)
	* CheXNet- Radiologist-Level Pneumonia Detection on Chest X-Rays with Deep Learning, 2018 吴恩达
	
* 检测(detection)
	* 医学图像
		* DeepRadiologyNet - Radiologist Level Pathology Detection in CT Head Images
		* 肺部CT图像病变区域检测方法
		* 基于定量影像组学的肺肿瘤良恶性预测方法
	* 自然图像
		* You Only Look Once- Unified, Real-Time Object Detection, CVPR 2016

* 增强(enhace)
	* 超分(super resolution)
		* Image Super-Resolution Using Deep Convolutional Networks
		* Deeply-Recursive Convolutional Network for Image Super-Resolution
* 分割(segmentation)
	* U-Net: Convolutional Networks for Biomedical Image Segmentation, 2015 MICCAI
	* A 3D Coarse-to-Fine Framework for Automatic Pancreas Segmentation

## 生成文字类任务
* 医学报告生成(medical report generation)
	* CNN-RNN
		* Learning to Read Chest X-Rays- Recurrent Neural Cascade Model for Automated Image Annotation, CVPR 2016
		* TieNet Text-Image Embedding Network for Common Thorax Disease Classification and Reporting in Chest X-rays, CVPR 2018[(author's homepage)](https://xiaosongwang.github.io)
		* On the Automatic Generation of Medical Imaging Reports, ACL 2018, CMU[(author's homepage)](http://www.cs.cmu.edu/~pengtaox/)
		* Multimodal Recurrent Model with Attention for Automated Radiology Report Generation, MICCAI 2018, PSU

	* Reinforcement Learning
		* Hybrid Retrieval-Generation Reinforced Agent for Medical Image Report Generation, NIPS 2018, CMU[(author's homepage)](https://www.cs.cmu.edu/~zhitingh/)
		
	* Other
		* TextRay Mining Clinical Reports to Gain a Broad Understanding of Chest X-rays, 2018

* 视觉描述生成(captioning)
	* Image Caption
		* CNN-RNN
			* Show, Attend and Tell: Neural Image Caption Generation with Visual Attention, ICML 2015[(code)](https://github.com/kelvinxu/arctic-captions)
			* Show and Tell: A Neural Image Caption Generator, CVPR 2015
			* Show and Tell: Lessons learned from the 2015 MSCOCO Image Captioning Challenge, PAMI 2016[(code)](https://github.com/tensorflow/models/tree/master/research/im2txt)
			* Areas of Attention for Image Captioning, ICCV 2017
			* (+)Rethinking the Form of Latent States in Image Captioning, ECCV 2018, CUHK
			* Recurrent Fusion Network for Image Captioning, ECCV 2018, Tencent AI Lab, 复旦
			
		* CNN-CNN
			* Convolutional Image Captioning, CVPR 2018([code](https://github.com/aditya12agd5/convcap))

		* Reinforcement Learning
			* Improving Reinforcement Learning Based Image Captioning with Natural Language Prior, 2018

		* Others
			* A Neural Compositional Paradigm for Image Captioning, NIPS 2018, CUHK

	* Video Caption
		* CNN-RNN
			* End-to-End Video Captioning with Multitask Reinforcement Learning
			* (+)Move Forward and Tell- A Progressive Generator of Video Descriptions, ECCV 2018, CUHK

* 视觉段落描述生成(visual paragraph description generation)
	* CNN-RNN
		* DenseCap: Fully Convolutional Localization Networks for Dense Captioning, CVPR 2016, Standford[(homepage)](https://cs.stanford.edu/people/karpathy/densecap/)[(code)](https://github.com/jcjohnson/densecap)
		* A Hierarchical Approach for Generating Descriptive Image Paragraphs, CVPR 2017[(homepage)](https://cs.stanford.edu/people/ranjaykrishna/im2p/index.html)[(dense-caption code)](https://github.com/InnerPeace-Wu/densecap-tensorflow)
		* Recurrent Topic-Transition GAN for Visual Paragraph Generation, ICCV 2017
		* Diverse and Coherent Paragraph Generation from Images, ECCV 2018[(code)](https://github.com/metro-smiles/CapG_RevG_Code)
		

* 视觉问答(visual question answering)
	* Image Question Answering
		* CNN-RNN
			* Multi-level Attention Networks for Visual Question Answering, CVPR 2017 
	
	* Video Question Answering
		* CNN-RNN
			* Motion-Appearance Co-Memory Networks for Video Question Answering, 2018
			* (++)Deep Attention Neural Tensor Network for Visual Question Answering, ECCV 2018, HIT



## 其它(others)
* Talk the Walk- Navigating New York City through Grounded Dialogue
* Generative Adversarial Nets, NIPS 2016
* Grounding Visual Explanations, ECCV 2018, UC Berkeley

