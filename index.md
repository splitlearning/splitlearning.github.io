# Split Learning Project Page: Distributed deep learning without sharing raw data #

**Abstract:** Split learning naturally allows for various configurations of cooperating entities to train (and infer from) machine learning  models without sharing any raw data or detailed information about the model. This method has been developed by the MIT Media Lab’s Camera Culture group.

<p align="center"> <a href=""><img src="https://splitlearning.github.io/diab1.png" height="320" width="600"></a></p>

**Key idea:** In the simplest of configurations of split learning, each client (for example, radiology center) trains a partial deep  network up to a specific layer known as the cut layer. The outputs at the cut layer are sent to another entity  (server/another client) which completes the rest of the training without looking at raw data from
any client that holds the raw data. This completes a round of forward propagation without sharing raw data. The gradients
are now back propagated again from its last layer until the cut layer in a similar fashion. The gradients at the
cut layer (and only these gradients) are sent back to radiology client centers. The rest of back
propagation is now completed at the radiology client centers. This process is continued until the
distributed split learning network is trained without looking at each others raw data.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=GiGlHuWOwME
" target="_blank"><img src="http://img.youtube.com/vi/GiGlHuWOwME/0.jpg" 
alt="Health Grid: Blockchain-based Data Marketplace | Ramesh Raskar | WEF 2019" width="240" height="180" border="10" /></a>     <a href="http://www.youtube.com/watch?feature=player_embedded&v=8GtJ1bWHZvg
" target="_blank"><img src="http://img.youtube.com/vi/8GtJ1bWHZvg/0.jpg" 
alt="RAMESH RASKAR INTERVIEW WITH BLOXLIVE AT THE WEF" width="240" height="180" border="10" /></a> <a href="http://www.youtube.com/watch?feature=player_embedded&v=7jWXaABY81I
" target="_blank"><img src="http://img.youtube.com/vi/7jWXaABY81I/0.jpg" 
alt="AI for All | Speedtalk | Ramesh Raskar" width="240" height="180" border="10" /></a>

## References
<b>Split Learning Papers: </b>

1.) Distributed learning of deep neural network over multiple agents, Otkrist Gupta and Ramesh Raskar, In: Journal of Network and Computer Applications 116, [(PDF)](https://www.sciencedirect.com/science/article/pii/S1084804518301590 "Pdf") (2018)

2.) Split learning for health: Distributed deep learning without sharing raw patient data, Praneeth Vepakomma, Otkrist Gupta, Tristan Swedish, Ramesh Raskar, [(PDF)](https://arxiv.org/pdf/1812.00564.pdf "Pdf") (2018)

3.) Survey paper: No Peek: A Survey of private distributed deep learning, Praneeth Vepakomma, Tristan Swedish, Ramesh Raskar, Otkrist Gupta, Abhimanyu Dubey, [(PDF)](https://arxiv.org/pdf/1812.03288.pdf "Pdf") (2018)

<b>AutoML Papers: </b>

1.) Accelerating neural architecture search using performance prediction, Bowen Baker, Otkrist Gupta, Ramesh Raskar, Nikhil Naik, In: conference paper at ICLR, [(PDF)](https://arxiv.org/pdf/1705.10823.pdf "Pdf") (2018)

2.) Designing neural network architecture using reinforcement learning, Bowen Baker, Otkrist Gupta, Nikhil Naik & Ramesh Raskar, In: conference paper at ICLR, [(PDF)](https://arxiv.org/pdf/1611.02167.pdf "Pdf") (2017)

## Come join us to learn more (CVPR Tutorial):
We are giving a half-day tutorial at CVPR 2019: 
On Distributed Private Machine Learning for Computer Vision: Federated Learning, Split Learning and Beyond

## Split learning's computational and communication efficiency on clients:
Client-side communication costs are significantly reduced as the data to be
transmitted is restricted to initial layers of the split learning network (splitNN) prior to the split. The
client-side computation costs of learning the weights of the network are also
significantly reduced for the same reason. In terms of model performance, the
accuracies of Split NN remained competitive to other distributed deep learning methods like federated learning and large
batch synchronous SGD with a drastically smaller client side computational
burden when training on a larger number of clients as shown below in terms of teraflops of computation and gigabytes of communication when split learning is used to train Resnet and VGG architectures over 100 and 500 clients with CIFAR 10 and CIFAR 100 datasets. 

<p align="center"><img src="https://splitlearning.github.io/splitTable.png" height="320" width="600"></p>
<p align="center"><img src="https://splitlearning.github.io/splitPlot.png" height="350" width="700"></p>

## Versatile plug-and-play configurations of split learning
Versatile configurations of split learning configurations cater to various practical settings of **i) multiple entities holding different modalities of patient data, ii) centralized and local health entities collaborating on
multiple tasks, iii) learning without sharing labels, iv) multi-task split learning, v) multi-hop split learning** and other hybrid possibilities to name a few as shown below and further detailed in our paper here [(PDF)](https://arxiv.org/pdf/1812.00564.pdf "Pdf")
<p align="center"><img src="https://splitlearning.github.io/splitConfig.png" height="400"></p><br />

## Slides on split learning for data transparent ML
<p align="center"><a href="https://www.slideshare.net/cameraculture/split-learning-versus-federated-learning-for-data-transparent-ml"><img src="https://splitlearning.github.io/splitSlides.png" align="center" height="350" width="600" ></a></p>

## News stories
**MIT Technology Review:** A new AI method can train on medical records without revealing patient data https://www.technologyreview.com/the-download/612567/a-new-ai-method-can-train-on-medical-records-without-revealing-patient-data/

**MIT Technology Review:** A little-known AI method can train on your health data without threatening your privacy https://www.technologyreview.com/s/613098/a-little-known-ai-method-can-train-on-your-health-data-without-threatening-your-privacy/

**MIT Technology Review:** The Algorithm Newsletter: The privacy-preserving AI technique that will transform healthcare
