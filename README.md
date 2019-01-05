# Anomaly-Detection
Week 1 Fundamentals of hypothesis testing, including the `null and alternative hypotheses`, `the test statistic` and the `p-value`, `power and the Neyman-Pearson lemma` <br>
Week 2 `Combining p-values`, including `Fisher’s, Stouﬀer’s, Simes’`, higher criticism and how you choose between them <br>
#### Fisher's combining p-values, Stouffer's combining p-values and Simes' combining p-values<br>
Week 3 Multiple testing, including `controlling false positives`, `the familywise error rate`, and `the false discovery rate` <br>
Week 4 Miscellanea, including `handling discrete test statistics`, `Bayesian p-values`, `Monte Carlo p-values`, and `connections to machine-learning` <br>
Weeks 4/5/6 Modelling dynamic network data: tractable and scalable Bayesian techniques. This will include three problem classes, and assessed coursework handed out in Week 4 and due by Thursday 20th December
## Chi square
符合某种分布，均值为多少，方差为多少，是对全体n个变量的三个约束，也是三个方程。所以本来n个自由度要减去3。
https://www.zhihu.com/question/22947034
假设你现在手头有 3 个样本X1 X2 X3，。因为样本具有随机性，所以它们取值不定。但是假设出于某种原因，我们需要让样本均值固定，比如说，mean(X)=5  ， 那么这时真正取值自由，”有随机性“ 的样本只有 2 个。 试想，如果mean确定 ,那么每选取一组X1 X2 的取值， X3将不得不等于15-X1-X2 对于第三个样本来说，这种 “不得不” 就可以理解为被剥夺了一个自由度。所以就这个例子而言，3 个样本最终"自由"的只有其中的 2 个。不失一般性，n个样本， 留出一个自由度给固定的均值，剩下的自由度即为n-1。
https://www.zhihu.com/question/20983193/answer/115599650

作者：DeviliveD
链接：https://www.zhihu.com/question/20983193/answer/28228799
来源：知乎
著作权归作者所有。商业转载请联系作者获得授权，非商业转载请注明出处。
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
Fisher's method: product of P values

Fisher’s method allows a majority (although perhaps not overwhelming) of tests to be inconclusive while still detecting an effect if there are a few, strong signals. For example:

Admissibility criterion (Birnbaum, 1954)
If H0 is rejected for any given set of pi , then it will also be rejected for all sets of pi∗ such that pi∗ ≤ pi for each i.
Theorem (Birnbaum, 1954)
For each method of combination satisfying the admissibility criterion, we can find some alternative H1 represented by non-increasing densities fi against which that method of combination gives a best test of H0.

### multiple_testing
### discrete_pvalues
### network_anomaly_detection
### Connections to machine-learning
### Network anomaly detection: the state of the art
