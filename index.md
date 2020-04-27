# Distributed deep learning and inference without sharing raw data #
## MIT Alliance for Distributed and Private Machine Learning 

**Abstract:** Friction in data sharing is a large challenge for large scale machine learning. Recently techniques such as Federated Learning, Differential Privacy and Split Learning aim to address siloed and unstructured data, privacy and regulation of data sharing and incentive models for data transparent ecosystems. Split learning is a new technique developed at the MIT Media Lab’s Camera Culture group that allows for participating entities to train machine learning models without sharing any raw data.

### New Program: MIT Alliance for Distributed and Private Machine Learning

The program will explore the main challenges in data friction that make capture, analysis and deployment of AI technologies.
The challenges include siloed and unstructured data, privacy and regulation of data sharing and incentive models for data transparent ecosystems. The research program with study automated machine learning (AutoML), privacy preserving machine learning (PrivateML) and intrinsic as well as extrinsic data valuation (Data Markets). By working with a stakeholder and innovator network, we aim to create a standard for data transparent ecosystems that can simultaneously address the privacy and utility of data. Our broad focus would be on key technologies such as **Differential privacy, Federated Learning and Split Learning.**<br/>

The program members will meet 4 times a year, publish case studies of AI on siloed data, will develop a curated github archive and engage in privacy aware data sharing protocol discussion towards a data exchange standard. We expect this integrated program to lead to many publications, training of talent, new technologies and standards.<br/>

MIT Media Lab consortium members can join the alliance as a special interest group SIG member. Non-member companies, startups and non-profits can join via undirected research gift. To know more about the program, please contact at <i>vepakom(at)mit.edu</i>

## New: COVID19 SafePaths Project at [(CovidSafePaths.org)](https://covidsafepaths.org/ "CovidSafePaths.org")
A global community-led movement
Safe Paths develops free, open-source, privacy-by-design tools for residents, public health officials, and larger communities to flatten the curve of COVID-19, reduce fear, and prevent a surveillance-state response to the pandemic.

**CovidSafePaths References**

1.) Apps Gone Rogue: Maintaining Personal Privacy in an Epidemic, 2020. [(PDF)](https://arxiv.org/abs/2003.08567 "Pdf")

2.) COVID-19 Contact-Tracing Mobile Apps: Evaluation and Assessment for Decision Makers, 2020. [(PDF)](https://drive.google.com/file/d/1A9Ft7-YpB9IOCbaLrRHrR34XP2SiSet5/view
 "Pdf")
 
3.)  Bluetooth based Proximity, Multi-hop Analysis and Bi-directional Trust: Epidemics and More, 2020. [(PDF)](https://www.researchgate.net/publication/340789081_Bluetooth_based_Proximity_Multi-hop_Analysis_and_Bi-directional_Trust_Epidemics_and_More
 "Pdf")

## Split Learning and Inference:

<p align="center"><a href="https://www.slideshare.net/cameraculture/split-learning-versus-federated-learning-for-data-transparent-ml"><img src="https://splitlearning.github.io/splitSlides.png" align="center" height="200" width="360" ></a></p>

Split learning removes barriers for collaboration in a whole range of sectors including healthcare, finance, security, logistics, governance, operations and manufacturing.
<p align="center"><a href=""><img src="https://splitlearning.github.io/diab1.png" height="320" width="600"></a></p>

For example, a split learning configuration as shown below allows for resource-constrained local hospitals with smaller individual datasets to collaborate and build a machine learning model that offers superior healthcare diagnostics, without sharing any raw data across each other as necessitated by trust, regulation and privacy.

<p align="center"><a href=""><img src="https://splitlearning.github.io/sl.png" height="320" width="600"></a></p>

**Landscape of related work:**
As shown below, split learning ideally fills the gap for being able to perform advanced AI tasks like training machine learning models in distributed settings with a substantial level of data protection.
<p align="center"><a href=""><img src="https://splitlearning.github.io/1.png" height="320" width="600"></a></p>


## Videos of Privacy aware AI, Split Learning at World Economic Forum and Niti Aayog
<a href="http://www.youtube.com/watch?feature=player_embedded&v=GiGlHuWOwME
" target="_blank"><img src="http://img.youtube.com/vi/GiGlHuWOwME/0.jpg"
alt="Health Grid: Blockchain-based Data Marketplace | Ramesh Raskar | WEF 2019" width="210" height="180" border="10" /></a>     <a href="http://www.youtube.com/watch?feature=player_embedded&v=8GtJ1bWHZvg
" target="_blank"><img src="http://img.youtube.com/vi/8GtJ1bWHZvg/0.jpg"
alt="RAMESH RASKAR INTERVIEW WITH BLOXLIVE AT THE WEF" width="210" height="180" border="10" /></a> <a href="http://www.youtube.com/watch?feature=player_embedded&v=7jWXaABY81I
" target="_blank"><img src="http://img.youtube.com/vi/7jWXaABY81I/0.jpg"
alt="AI for All | Speedtalk | Ramesh Raskar" width="210" height="180" border="10" /></a>
<a href="https://www.youtube.com/watch?v=hHV2WR7nCQk
" target="_blank"><img src="http://img.youtube.com/vi/hHV2WR7nCQk/0.jpg"
alt="Ramesh Raskar: UNC-Chapel Hill Convocation Speaker | 2019" width="210" height="180" border="10" /></a>
<br />
<a href="https://www.youtube.com/watch?v=x9TCYuMUnco
" target="_blank"><img src="http://img.youtube.com/vi/x9TCYuMUnco/0.jpg"
alt="Ramesh Raskar: TEDxBeaconStreet | 2019" width="210" height="180" border="10" /></a>
<a href="https://www.youtube.com/watch?v=4PdBM76D5JY
" target="_blank"><img src="http://img.youtube.com/vi/4PdBM76D5JY/0.jpg"
alt="Ramesh Raskar: UNC-Chapel Hill Convocation Speaker | 2019" width="210" height="180" border="10" /></a>
<br />


**Key technical idea:** In the simplest of configurations of split learning, each client (for example, radiology center) trains a partial deep  network up to a specific layer known as the cut layer. The outputs at the cut layer are sent to another entity  (server/another client) which completes the rest of the training without looking at raw data from
any client that holds the raw data. This completes a round of forward propagation without sharing raw data. The gradients
are now back propagated again from its last layer until the cut layer in a similar fashion. The gradients at the
cut layer (and only these gradients) are sent back to radiology client centers. The rest of back
propagation is now completed at the radiology client centers. This process is continued until the
distributed split learning network is trained without looking at each others raw data.<br />
## SplitNN Architectures, Leakage Prevention and Diverse Applications
<p align="center"><a href=""><img src="https://splitlearning.github.io/boomerang.png" height="190" width="220"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href=""><img src="https://splitlearning.github.io/alicebob.png" height="190" width="220"></a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href=""><img src="https://splitlearning.github.io/noPeek1.png" height="190" width="220">
</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href=""><img src="https://splitlearning.github.io/recons.png" height="190" width="220">
</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href=""><img src="https://splitlearning.github.io/colorectal.png" height="190" width="220">
</a>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href=""><img src="https://splitlearning.github.io/health_data.png" height="190" width="220"></a>
</p>

## Potential Partner/Want to connect with us?
Please fill this simple [form](https://forms.gle/C7dX8ynRsre4xYdP8 "form") to reach out

<h2 id="faq"> Frequently asked questions </h2>

1. **How does split learning work and what is new in our approach?** <br />
    Split learning attains high resource efficiency for distributed deep learning in comparison to existing methods by splitting the models architecture across distributed entities. It only communicates activations and gradients just from the split layer unlike other popular methods that share weights/gradients from all the layers. Split learning requires no raw data sharing; either of labels or features.


2. **How is raw data protected and who can get positively impacted?**<br />
    Split learning requires absolutely no raw data sharing. Sectors like healthcare, finance, security, surveillance and others where data sharing is prohibited will benefit from our approach for training distributed deep learning models. Another modality of split learning called NoPeek SplitNN also drastically reduces leakage due to any communicated activations by reducing their distance correlation with raw data while maintaining model performance via categorical cross-entropy.


3. **How long will it take to transition from laboratory setting to actual deployments between cooperating entities?**<br />
	The approach is easily deployable for inter and intra entity or organizational collaboration and is highly versatile in terms of possible network topologies. Due to its high resource efficiency in terms of computations, memory, communication bandwidth it is also naturally suitable for distributed learning where the clients are pervasive and ubiquitous edge devices like mobile phones or IOT devices as well as across larger devices and organizations.
<br /><br />

## References
<b>Split Learning Papers: </b>

1.) Distributed learning of deep neural network over multiple agents, Otkrist Gupta and Ramesh Raskar, In: Journal of Network and Computer Applications 116, [(PDF)](https://www.sciencedirect.com/science/article/pii/S1084804518301590 "Pdf") (2018)

2.) Reducing leakage in distributed deep learning for sensitive health data, Praneeth Vepakomma, Otkrist Gupta, Abhimanyu Dubey, Ramesh Raskar, Accepted to ICLR 2019 Workshop on AI for social good.[(PDF)](https://aiforsocialgood.github.io/iclr2019/accepted/track1/pdfs/29_aisg_iclr2019.pdf "Pdf") (2019)

3.) Split learning for health: Distributed deep learning without sharing raw patient data, Praneeth Vepakomma, Otkrist Gupta, Tristan Swedish, Ramesh Raskar, Accepted to ICLR 2019 Workshop on AI for social good.[(PDF)](https://arxiv.org/pdf/1812.00564.pdf "Pdf") (2018)

4.) Detailed comparison of communication efficiency of split learning and federated learning, Abhishek Singh, Praneeth Vepakomma, Otkrist Gupta, Ramesh Raskar, [(PDF)](https://arxiv.org/pdf/1909.09145.pdf "Pdf") (2019)

5.) ExpertMatcher: Automating ML Model Selection for Users in Resource Constrained Countries, Vivek Sharma, Praneeth Vepakomma, Tristan Swedish, Ken Chang, Jayashree Kalpathy-Cramer, and Ramesh Raskar [(PDF)](https://arxiv.org/pdf/1910.02312.pdf "Pdf") (2019)

6.) Split Learning for collaborative deep learning in healthcare, Maarten G.Poirot, Praneeth Vepakomma, Ken Chang, Jayashree Kalpathy-Cramer, Rajiv Gupta, Ramesh Raskar (2019)

<b>Survey Papers: </b>

1.) Advances and open problems in federated learning (with, 58 authors from 25 institutions!) [(PDF)](https://arxiv.org/pdf/1912.04977.pdf "Pdf") (2019)

2.) No Peek: A Survey of private distributed deep learning, Praneeth Vepakomma, Tristan Swedish, Ramesh Raskar, Otkrist Gupta, Abhimanyu Dubey, [(PDF)](https://arxiv.org/pdf/1812.03288.pdf "Pdf") (2018)

3.) A Review of Homomorphic Encryption Libraries for Secure Computation, Sai Sri Sathya, Praneeth Vepakomma, Ramesh Raskar, Ranjan Ramachandra, Santanu Bhattacharya, [(PDF)](https://arxiv.org/pdf/1812.02428.pdf "Pdf") (2018)

<b>AutoML Papers: </b>

1.) Accelerating neural architecture search using performance prediction, Bowen Baker, Otkrist Gupta, Ramesh Raskar, Nikhil Naik, In: conference paper at ICLR, [(PDF)](https://arxiv.org/pdf/1705.10823.pdf "Pdf") (2018)

2.) Designing neural network architecture using reinforcement learning, Bowen Baker, Otkrist Gupta, Nikhil Naik & Ramesh Raskar, In: conference paper at ICLR, [(PDF)](https://arxiv.org/pdf/1611.02167.pdf "Pdf") (2017)

## Upcoming: CVPR 2019 Half-Day Tutorial on “Distributed Private Machine Learning for Computer Vision: Federated Learning, Split Learning and Beyond” [(Link)](https://nopeekcvpr.github.io/ "Link").
We are giving a half-day tutorial at CVPR 2019:
On Distributed Private Machine Learning for Computer Vision: Federated Learning, Split Learning and Beyond by
<b> Brendan McMahan (Google, USA)</b>, <b>Jakub Konečný</b> (Google, USA), <b>Otkrist Gupta (LendBuzz)</b>, <b>Ramesh Raskar</b> (MIT Media Lab, Cambridge, Massachusetts, USA),<b> Hassan Takabi</b> (University of North Texas, Texas, USA) and <b>Praneeth Vepakomma</b> (MIT Media Lab, Cambridge, Massachusetts, USA).
<br />
## Recent talk on Split Learning at Datacouncil.ai SF 2019 [(Slides)](splitlearning.github.io/Split-Learning-A-Resource-Efficient-Distributed-Deep-Learning-Method-Without-Sensitive-Data-Sharing.pdf "Slides")

## Recent course on Advances in imaging and machine learning: Medical, VR-AR, And Self-Driving Cars [(Link)](https://professional.mit.edu/programs/short-programs/advances-imaging "Link")

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

## News stories
1. [(A new AI method can train on medical records without revealing patient data)](https://www.technologyreview.com/the-download/612567/a-new-ai-method-can-train-on-medical-records-without-revealing-patient-data/ "A new AI method can train on medical records without revealing patient data")

2. [(A little-known AI method can train on your health data without threatening your privacy)](https://www.technologyreview.com/s/613098/a-little-known-ai-method-can-train-on-your-health-data-without-threatening-your-privacy/ "A little-known AI method can train on your health data without threatening your privacy")

3. [(The Algorithm Newsletter: The privacy-preserving AI technique that will transform healthcare)](https://go.technologyreview.com/the-privacy-preserving-machine-learning-technique-that-will-transform-healthcare "The Algorithm Newsletter: The privacy-preserving AI technique that will transform healthcare")

4. [(Les Echos: Medical secrecy, artificial intelligence and RGPD: irreconcilable? Not so sure…)](https://www.lesechos.fr/idees-debats/cercle/opinion-secret-medical-intelligence-artificielle-et-rgpd-irreconciliables-pas-si-sur-999364 "Les Echos: Medical secrecy, artificial intelligence and RGPD: irreconcilable? Not so sure…")

**Team**<br/>
Ramesh Raskar, Associate Professor, MIT Media Lab; Principal Investigator<br/>
Praneeth Vepakomma, MIT<br/>
Abhishek Singh, MIT<br/>
Otkrist Gupta, MIT Affiliate<br/>
Vitor Pamplona, MIT Affiliate<br/>
Kevin Pho, MIT<br/>

MIT Alliance for Distributed and Private Machine Learning

## Potential Partner/Want to connect with us?
Please fill this simple [form](https://forms.gle/C7dX8ynRsre4xYdP8 "form") to reach out
