

![cover](https://ws1.sinaimg.cn/large/006tNc79gy1fn924jmcfmj31dc0h8js4.jpg)

![Contributions Welcome](https://img.shields.io/badge/Contributions-welcome-blue.svg)

Know a resource that isn't listed below? Feel free to create a new [pull request](https://github.com/fateleak/awesome-chatbot-list/pulls), or open an [issue](https://github.com/fateleak/awesome-chatbot-list/issues/new).Seq2seq/chatbot/聊天机器人相关资源收集列表。

在原来的chatbot-links的基础上，添加了一些更多的中文资源而组建的一个List，主要用于个人收集。感兴趣，一起建设完善的资源列表，方便萌新入门，请发送PR或Issue添加更多资源，各层面不限，欢迎添加自己的作品。



___

## Codes

#### [chatbot-rnn](https://github.com/pender/chatbot-rnn)

Framework tensorflow

A toy chatbot powered by deep learning and trained on data from Reddit.

```
> Hi, how are you?
 I'm not the only one here that's having fun with you, it's all me.
> Who else is with you?
 Haha. I'm not the one who made the comment. I'm the one who said that and didn't think that much of anything. 
> Oh, I see. So what's new?
 Nothing. I just thought it was a bit of an overreaction. It's been a while since I've read it. 
> It's all good
 It's all good. It's one of those things that makes me smile :)
> That's great. This is actually my demo chat, so it's nice that you're keeping things positive!
 Thank you :) 
```


#### [DeepQA](https://github.com/Conchylicultor/DeepQA)

Framework: Tensorflow
Demo result:

    Hi			            	→ Hi.
    What is your name ?			→ Laura.
    What does that mean ?		→ I dunno.
    How old are you ?			→ thirty-five.
    Who is Laura ?				→ My brother.
    Say 'goodbye'				→ Alright.
    Two plus two				→ manny...

#### [tf_seq2seq_chatbot](https://github.com/nicolas-ivanov/tf_seq2seq_chatbot)
Framework: Tensorflow

No answering randomisation is implemented in this code, so the models answers with the same phrase way each time:
未实现回答的是随机化，仅对模型的末尾加入了稀疏层。

    hello baby					→ hello
    how old are you ?			→ twenty .
    i am lonely					→ i am not
    nice						→ you ' re not going to be okay .
    so rude						→ i ' m sorry .
    are you a robot or human?	→ no .
    are you better than siri?	→ yes .

####  [machine translation model](https://github.com/tensorflow/tensorflow/tree/master/tensorflow/models/rnn/translate)

Framework: Tensorflow

Google Official seq2seq implementation, attention included. Originlly for translation, can be used as Q/A;
Google官方的seq2seq实现，采用了注意力机制(Luong et al., 2015)，原本用于语言翻译，也适用于简单Q/A。
![](https://ws2.sinaimg.cn/large/006tNc79gy1fn924qhmvtj30ck09cdia.jpg)



#### [Neural-Dialogue-Generation](https://github.com/jiweil/Neural-Dialogue-Generation)
Framework: Torch 6.x
Source code for a bunch of super nice articles by Jiwei Li - one of my favorite researches in the domain of neural conversational systems. Worth checking out.

    tell me ... how long have you had this falling sickness ?       → a few months, I guess .
    so i had the doctors test sammy ’s response to conditioning .   → so he took the pills .
    what are you going to do ?                                      → i ’m going to get you a new car .
    they fear your power your intellect .                           → i ’m not afraid of your power .

#### [neuralconvo](https://github.com/macournoyer/neuralconvo)

Framework: Torch 7

最早的对《A Neural Conversational Model》的实现之一，当时给的Demo效果非常有意思。

    Hello?					→ Hi.
    How are you?			→ I'm fine.
    What's your name?		→ It's hard to describe.
    How so?					→ I'm not sure.
    What color is the sky?	→ It's blue.
    What is your job?		→ It's not that i'm a fucking werewolf!

#### [chatbot-zh-torch7](https://github.com/fateleak/chatbot-zh-torch7)

Framework: Torch 7

从neuralconvo修改而来的，当时应该是第一个中文的RNN based chatbot DEMO。
![chatbot-zh-torch7](https://ws1.sinaimg.cn/large/006tNc79gy1fn924y5hjvj30il0dwmz8.jpg)

####  [Seq2seq_Chatbot_QA](https://github.com/qhduan/Seq2Seq_Chatbot_QA)
Framework: Tensorflow
一个中文的Demo，说明比较详细，推荐。

result:

	你到哪里去        →你不是说你不是我的
	你喜欢我吗？      →我喜欢你
	你吃了吗？        →我还没吃饭呢
	你喜欢喝酒吗？     →我不知道
	你说话没有逻辑啊   →没有

#### [ChatterBot](https://github.com/gunthercox/ChatterBot)

Framework: python

看上去比较完整的一个项目，安装简单，说明比较完善，有提供训练的材料，英文为主。

	Good morning! How are you doing?   →I am doing very well, thank you for asking.
	You're welcome.                    →Do you like hats?



#### [farizrahman4u/seq2seq](https://github.com/farizrahman4u/seq2seq)

#### [nicolas-ivanov/debug_seq2seq](https://github.com/nicolas-ivanov/debug_seq2seq)
#### [codekansas/keras-language-modeling](https://github.com/codekansas/keras-language-modeling)
Framework: keras


这几个都是seq2seq的实现，但是在Chatbot上面还没有好的demo result。

#### [oswaldoludwig/Seq2seq-Chatbot-for-Keras](https://github.com/oswaldoludwig/Seq2seq-Chatbot-for-Keras)
A new generative chatbot whose training converges in few epochs, including a model pre-trained on a small but consistent dataset collected from dialogues of English courses online.

这个采用了生成模型的方式，待补充。

        user:  Hello! How are you?
    computer:  i am fine , ok , well , thank you  .  
    
        user:  What's your name?
    computer:  janet .   
    
        user:  What do you like to do now?
    computer:  let me think a minute .   
    
        user:  I want to chat about computer science.
    computer:  i am glad to hear there .   
    
        user:  Are you a real girl or a computer program?
    computer:  i am self employed . i would love to be well .   
    
        user:  Why don't you look for a job?
    computer:  i do not know . i am the bank .   
    
        user:  So, you don't need a job!
    computer:  no . i have to make a lot of money .  



### [pydial](http://www.camdial.org/pydial/)

一个多领域多轮会话的开发框架

![](r/1.png)
[paper](http://www.aclweb.org/anthology/P17-4013)

- 剑桥的开源DS [PyDial](http://www.camdial.org/pydial/)
- 一个开源的DS [deepmipt/DeepPavlov](https://github.com/deepmipt/DeepPavlov)
- 一个商业但开源的DS [Rasa Core](https://rasa.com/)
- 比较简单的机器人[ChatterBot](https://github.com/gunthercox/ChatterBot)
- 一个开源的QA系统，里面那个论文列表不错 [castorini/BuboQA](https://github.com/castorini/BuboQA)
- AIML的公司 [pandorabots](https://home.pandorabots.com/en/)

### 


## Corpus

#### [AlJohri/OpenSubtitles](https://github.com/AlJohri/OpenSubtitles)
Get a lot of raw movie subtitles (~1.2Gb)

#### [Cornell Movie-Dialogs Corpus](http://www.cs.cornell.edu/~cristian/Cornell_Movie-Dialogs_Corpus.html)
~ 40Mb after clearing out the technical data.

#### [dgk_lost_conv](https://github.com/fateleak/dgk_lost_conv)
[中文]语料。大部分为由字幕生成的材料，少量其它对话(如以前的小黄鸡的材料，我从一位网友朋友那里要过来了，感谢他)。
其中results/xiaohuangji50w_fenciA.conv.zip为上面chatbot-zh-torch7的演示的训练材料。

#### [原射手网的打包字幕合集17G]
现已关闭的射手网有一个所有字幕的合集包，感兴趣的同学需要自行网上搜索下载。

#### [Some English QA Material](https://github.com/karthikncode/nlp-datasets)
这是他人收集的自然语言处理相关数据集，主要包含Question Answering，Dialogue Systems， Goal-Oriented Dialogue Systems三部分，都是英文文本。可以使用机器翻译为中文，供中文对话使用。


#### TODO

dgk_lost_conv中字幕生成的材料的问题是质量较差，这是因为字幕文件中包含了很多的旁白，或者单人连续说话的情况，而这些在处理的时候都没有剔除掉。希望有同学能够找到方法。
或者
从微博、QQ群、微信群等地方挖掘更多的1v1的对话材料。


## Papers

* [\[1\] Sequence to Sequence Learning with Neural Networks][1]
* [\[2\] A Neural Conversational Model][2]

[1]: http://papers.nips.cc/paper/5346-sequence-to-sequence-learning-with-neural-networks.pdf
[2]: http://arxiv.org/pdf/1506.05869v1.pdf

## 其它：

为了方便中文用户中对chatbot/NLP/DeepLearning感兴趣的朋友们互相交流，建了一个QQ群，欢迎您加入讨论：

![chatbot_qq_qun](https://ws2.sinaimg.cn/large/006tNc79gy1fn925c4kmtj30k1082q3l.jpg)

[Github fork](https://github.com/fateleak/awesome-chatbot-list)
