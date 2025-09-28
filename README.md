<img width="1590" height="544" alt="image" src="https://github.com/user-attachments/assets/a08f1f3e-8093-4a6c-87a2-b5f022c6d4fb" />

# paper
我近期阅读的论文
## ITN
1. 1996 [Multilingual Text Analysis for Text-to-Speech Synthesis](https://arxiv.org/pdf/cmp-lg/9608012)这是一篇古老的论文，用有限状态自动机的方法解决文本标准化的问题。它提出了一种基于加权有限状态转换器（WFSTs）的模型，为多数文本标准化问题提供了统一的解决框架。

## 纠错
1. 2024 [Denoising LM: Pushing the Limits of Error Correction Models for Speech Recognition](https://arxiv.org/pdf/2405.15216) 这篇文章用大模型对语音识别的结果进行了纠错。纠错语料对来自于：先拿正确文本输入到TTS系统，再拿得到的音频输入ASR系统得到语音识别结果，这样就得到了纠错语料对了。
2. 2023 引用量79 [GENERATIVE SPEECH RECOGNITION ERROR CORRECTION WITH LARGE LANGUAGE MODELS AND TASK-ACTIVATING PROMPTING](https://assets.amazon.science/77/26/6c265e0a42d7a40d2ee8bdd158e6/generative-speech-recognition-error-correction-with-large-language-models-and-task-activating-prompting.pdf) 这篇论文首次使用prompt工程队第一遍ASR的N-best输出进行重打分从而实现纠错。由于年代比较早，以至于里面用的大模型居然还有GPT-2。从论文中可以看到，随着模型参数量的增加，纠错的效果越明显。
3. 2023 引用量77 [Can Generative Large Language Models Perform ASR Error Correction?](https://arxiv.org/pdf/2307.04172) 这也是一篇用n-best候选结果给chatGPT，让chatGPT来得到纠错结果。他们发现仅给最优的ASR结果给大模型，纠错效果并不好。
4. 2024 引用量8 [Evolutionary Prompt Design for LLM-Based Post-ASR Error Correction](https://arxiv.org/pdf/2407.16370) 这篇文章其实一直就是在优化prompt，看看哪个prompt更好，更能产生更好的纠错效果

## 智能体
1. [Exploring the Impact of Instruction Data Scaling on Large Language Models:
An Empirical Study on Real-World Use Cases](https://arxiv.org/pdf/2303.14742)
2. [STITCH: Simultaneous Thinking and Talking with Chunked Reasoning for Spoken Language Models
](https://arxiv.org/abs/2507.15375?context=eess.AS)

## 标点
1. 2011 IWSLT 引用量104 [Modeling Punctuation Prediction as Machine Translation](https://aclanthology.org/2011.iwslt-papers.7.pdf)
2. 2020 ICASSP 引用量54 [Controllable Time-Delay Transformer for Real-Time Punctuation Prediction and Disfluency Detection](https://arxiv.org/pdf/2003.01309)达摩院写的文章。把标点和顺滑联合建模。
3. 2019 ICASSP [Self-attention based model for
punctuation prediction using word and speech embeddings](https://www.researchgate.net/profile/Jianhua-Tao/publication/332791674_Self-attention_Based_Model_for_Punctuation_Prediction_Using_Word_and_Speech_Embeddings/links/640899e6574950594576ca5a/Self-attention-Based-Model-for-Punctuation-Prediction-Using-Word-and-Speech-Embeddings.pdf)
4. 2016 第十届语言资源与评价国际会议论文集:[Punctuation Prediction for Unsegmented Transcript Based on Word Vector](https://aclanthology.org/L16-1103.pdf)


## 人脸
人机面部协同表达
https://yuhang-hu.com/
1. [Human-robot facial coexpression](http://www.generalroboticslab.com/assets/files/coexpression.pdf)
2. [Teaching robots to build simulations of themselves](https://arxiv.org/pdf/2311.12151)
3. [Egocentric visual self-modeling for
autonomous robot dynamics prediction
and adaptation](https://www.nature.com/articles/s44182-025-00031-6.pdf)
胡宇航把一面镜子放到人脸机器人的面前。通过眼睛里的摄像头，机器人能将电机指令和脸部表情相对应，汇总给AI模型，再对照互联网数据，解读不同表情的意义，构建起语音、语义、表情间的联系。
“先借助互联网数据训练AI模型，再结合对镜收集的物理数据，通过自监督学习不断进化出对身体的理解，让机器人的表情更加精细，在不同语境下自主交互。”胡宇航介绍道。
此外，由于人脸是无数微动作的耦合，为了让人脸机器人更加逼真，必须在柔软、非线性的硅胶皮肤内塞进更多电机，以实现精准调控，同时不能破坏面部结构，为此胡宇航费了好大一番功夫。
“光是废弃的‘脸皮’就塞满了一整箱。”胡宇航说，现在他开发的最新人脸机器人已装进30个电机，足以支撑高精细度的表情，“但要做得更好，还得进一步提升工程能力”。
找不到同行者，胡宇航决定自己摸黑前进。“没有现成的基座，必须自己搭建；硅胶材料不稳定、易破损；人脸仿生的高曲面参数无法用传统的CAD软件建模；在优化动作的基础上还要设计、维护外观……”胡宇航语速越来越快，没有参考文献，没有工程先例，从算法、模型的开发，到实物的搭建、调优，全靠他一个人。
他常常一个人窝在实验室，3D打印出零部件，跑代码、建模型、搭实物，失败了几十次后，他多了两个“搭子”——“冷酷”和“冷漠”，一个登上了《科学-机器人学》，一个参与了科幻电影Posthuman的拍摄
