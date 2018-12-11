# Split Learning Project Page: Distributed deep learning without sharing raw data
<a href=""><img src="https://splitlearning.github.io/diab1.png" align="left" height="400" width="650" >

Split learning naturally allows for various configurations of cooperating entities to train (and infer from) machine learning  models without sharing any raw data or detailed information about the model. 
<br /><br /> In the simplest of configurations of split learning, each client (for example, radiology center) trains a partial deep  network up to a specific layer known as the cut layer. The outputs at the cut layer are sent to another entity   (server/another client) which completes the rest of the training without looking at raw data from
 any client that holds the raw data. This completes a round of forward propagation without sharing raw data. The gradients
 are now back propagated again from its last layer until the cut layer in a similar fashion. The gradients at the
 cut layer (and only these gradients) are sent back to radiology client centers. The rest of back
 propagation is now completed at the radiology client centers. This process is continued until the
 distributed split learning network is trained without looking at each others raw data.

## Split Learning Papers:

1.) “Distributed learning of deep neural network over multiple agents”, Otkrist Gupta and Ramesh Raskar, In: Journal of Network and Computer Applications 116, [(PDF)](https://www.sciencedirect.com/science/article/pii/S1084804518301590 "Pdf") (2018)

2.) Split learning for health: Distributed deep learning without sharing raw patient data, Praneeth Vepakomma, Otkrist Gupta, Tristan Swedish, Ramesh Raskar [(PDF)](https://arxiv.org/pdf/1812.00564.pdf "Pdf") (2018)

3.) Survey paper: No Peek: A Survey of private distributed deep learning, Praneeth Vepakomma, Tristan Swedish, Ramesh Raskar, Otkrist Gupta, Abhimanyu Dubey, [(PDF)](https://arxiv.org/pdf/1812.03288.pdf "Pdf") (2018)

## Slides on split learning versus federated learning for data transparent ML
<a href="https://www.slideshare.net/cameraculture/split-learning-versus-federated-learning-for-data-transparent-ml"><img src="https://splitlearning.github.io/splitSlides.png" align="left" height="400" width="600" ></a><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br /><br />


## Split learning's computational and communication efficiency on clients:
![](https://splitlearning.github.io/splitTable.png)
![Image of split example](https://splitlearning.github.io/splitPlot.png)

## Versatile plug-and-play configurations of split learning
![Split learning configurations](https://splitlearning.github.io/splitConfig.png)
Versatile configurations of split learning configurations cater to various practical settings of i) multiple entities holding different modalities of patient data, ii) centralized and local health entities collaborating on
multiple tasks, iii) learning without sharing labels, iv) multi-task split learning, v) multi-hop split learning and other hybrid possibilities to name a few as shown below and further detailed in our paper here [(PDF)](https://arxiv.org/pdf/1812.00564.pdf "Pdf")


