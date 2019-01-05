# Anomaly-Detection
Week 1 Fundamentals of hypothesis testing, including the `null and alternative hypotheses`, `the test statistic` and the `p-value`, `power and the Neyman-Pearson lemma` <br>
Week 2 `Combining p-values`, including `Fisher’s, Stouﬀer’s, Simes’`, higher criticism and how you choose between them <br>
#### Fisher's combining p-values, Stouffer's combining p-values and Simes' combining p-values<br>
Week 3 Multiple testing, including `controlling false positives`, `the familywise error rate`, and `the false discovery rate` <br>
Week 4 Miscellanea, including `handling discrete test statistics`, `Bayesian p-values`, `Monte Carlo p-values`, and `connections to machine-learning` <br>
Weeks 4/5/6 Modelling dynamic network data: tractable and scalable Bayesian techniques. This will include three problem classes, and assessed coursework handed out in Week 4 and due by Thursday 20th December

## Topics
### Why anomaly detection
ILO1 To recognise and apply a range of models for dynamic network data, and their estimation <br>
ILO2 To understand core anomaly detection concepts and tools, including `mastering theory` and `interpretation of hypothesis tests`, `controlling false positive rates` and `performing meta-analysis` <br>
ILO3 To apply these anomaly detection tools to analyse real large-scale data and report the result<br>
<br>
EXAM: ILO1 AND ILO2 <br>

### Hypothesis testing fundamentals
#### Null and alternative hypotheses
H0 H1 hypotheses
https://www.icourse163.org/learn/UESTC-1001590004?tid=1003273003#/learn/content?type=detail&id=1004590602&cid=1005781829
#### Test statistic
T is a real-valued function of the data T = g(D), which is used to decide which hypothesis is true.

#### The p-value
p, associated with the observed value of a test statistic, t, is the probability under the null of observing a test statistic as extreme as t
观察一个极端的测试统计量的概率
所以p value 是一个与观测统计量t有关的一个概率，这个概率是一个t在极端状态下的概率

##### Distribution of the p-value under the null hypothesis
Assume the test statistic T has a continuous distribution. Then, under the null hypothesis, the p-value is uniformly distributed on [0,1].
**** How to proof!!
##### Rejecting the null hypothesis
##### Power
 the power of a hypothesis test is the probability of rejecting the null hypothesis if the alternative holds: 
 ```P(Reject H0 | H1 holds) = P1(Reject H0). ```
##### Increasing functions of a test statistic

Consider test statistics T1, T2 satisfying T2 = h(T1) where h is a strictly increasing function. Let t1, t2 be the observed values of T1, T2. Then the p-values p1, p2 associated with t1, t2 are equal.
 
##### The Neyman-Pearson Lemma
 台湾公开课有帮助但是特别长：http://ctld.video.nccu.edu.tw/media/752

 youtube上一个视频感觉不错：https://www.youtube.com/watch?v=UJnUrMMmrFU
##### Distribution of the p-value under the alternative
##### Other tests


### combining_pvalues
### multiple_testing
### discrete_pvalues
### network_anomaly_detection
### Connections to machine-learning
### Network anomaly detection: the state of the art
