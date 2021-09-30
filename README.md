# Learning_web

## Imitation Learning
* [介绍](https://cloud.tencent.com/developer/article/1144328)

---

## Fog computing & Edge computing

![img](./pics/01.jpg)

### !!! fog computing can’t replace edge computing. However, edge computing can definitely live without fog computing

### Fog computing
1. efficiency of data traffic and a reduction in latency
2. lower storage need
3. faster data transfer
4. requires an investment. It is a more complex system

### Edge computing

> edge computing happens where data is being generated, right at “the edge” of a given application’s network. This means that an edge computer is connected to the sensors and controllers of a given device and then sends data to the cloud. 

---

## Software Defined Space-Air-Ground Integrated Vehicular Networks

> 各取好處，在都市使用地面網路(RSU)到了不密集的鄉村則善用衛星。

![img](./pics/02.jpg)

>Ref. Software Defined Space-Air-Ground 
Integrated Vehicular Networks:
Challenges and Solutions

---

## 馬可夫決策過程 Markov Decision Process（MDP）

> 只要是連續決策、而且在決策過程中的行動具有不確定性，就可以用 MDP 來處理。
[!!!連結!!!](https://blog.techbridge.cc/2018/10/27/intro-to-mdp-and-app/)


---
## 卜松過程 (Poisson Process)
>卜松過程是馬可夫過程 (Markov Proscess) 中最簡單的一種
1. [!!!連結!!!](http://episte.math.ntu.edu.tw/articles/mm/mm_02_4_01/index.html)
2. [證明影片](https://www.youtube.com/watch?v=Cd1r98qABl8&t=1s)

---
## 馬可夫鏈（Markov chain）
>一狀態的機率分布只能由當前狀態決定，在時間序列中它前面的事件均與之無關。這種特定類型的「無記憶性」稱作馬可夫性質
[!!!連結!!!](http://episte.math.ntu.edu.tw/articles/mm/mm_09_3_08/page2.html)

---

## Markov-modulated Poisson Process (MMPP)

>Poisson process that has its parameter controlled by a Markov process. These arrival processes are typical in communications modeling where time-varying arrival rates capture some of the important correlations between inter-arrival times. 
[!!!連結!!!](https://www.sfu.ca/sasdoc/sashtml/qsim/chap9/sect7.htm)

* [契約理論（Contract_Theory）](https://wiki.mbalib.com/zh-tw/%E5%A5%91%E7%BA%A6%E7%90%86%E8%AE%BA)
* [前景理論(Prospect_Theory)](https://wiki.mbalib.com/zh-tw/%E5%89%8D%E6%99%AF%E7%90%86%E8%AE%BA)

---

## 排隊理論 (queueing)

### 歷史
>厄朗（英語：Agner Krarup Erlang）（Agner Krarup Erlang）一個在丹麥哥本哈根電話交換局工作的工程師，研究人們打電話的方式，發展出人們需要等待多久的公式，並於1909年出版了關於排隊理論的第一篇論文[5]。

### 表示法

* A/B/C/X/Y/Z
* A-到達的規則；
* B-服務規則，即指服務時間（相當於報文發送時間）的長短服從什麼規律；
* C-服務台個數
* X-模型中平行的隊列（即服務通道或發送信道）數目；
* Y-系統流量限制
  

Z的符號有以下類型

* FCFS 先來先服務
* LCFS 後來先服務
* RSS 隨機選擇哪個先服務
* PR 由優先權決定
* GD 通用規則


![img](./pics/03.jpg)

### 常見

> 我們會常常省去後兩個位置[ A/B/C ]，默認為系統無容納上限，先到先服務原則。如非常經典又基礎的 M/M/1 及 M/M/S 模型 (顧客抵達與服務時間均為指數分佈，一個或多個服務台).



1. [排队论](https://zhuanlan.zhihu.com/p/99131787) 
2. [等候理論](https://www.wikiwand.com/zh-hk/%E7%AD%89%E5%80%99%E7%90%86%E8%AB%96)



