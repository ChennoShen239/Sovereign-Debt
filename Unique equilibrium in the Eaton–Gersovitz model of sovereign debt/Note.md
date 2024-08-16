### Highlights 亮点

- The Eaton–Gersovitz model is widely used for empirical analyses of sovereign debt markets.  
  - Eaton–Gersovitz 模型被广泛用于主权债务市场的实证分析。

- We show that the model with exogenous default value and short-term debt admits a unique equilibrium.  
  - 我们表明，具有外生违约值函数和短期债务的模型存在唯一均衡。

- This counters the common view that sovereign debt markets are prone to multiple equilibria.  
  - 这反驳了主权债务市场容易陷入多重均衡的普遍观点。

- Multiplicity requires altering the timing of the model, or considering long-term debt.  
  - 多元性需要调整模型的时序或考虑长期债务。

In this paper we explain why, by proving that equilibrium is _unique_ in the benchmark infinite-horizon model with a Markov process for the exogenous driving state and exogenous value from default.

在本文中，我们通过证明在基准无限期界模型中，对于外生驱动状态和外生违约价值具有马尔可夫过程的均衡是唯一的，来解释了这一点

为什么我们研究的基准模型中会出现多重性？为了建立直观，考虑最简单的环境：债务被限制为无风险，如张（1997）所述。该模型的马尔可夫完美均衡特征是（恒定的）内生债务上限，这是今天可以承担的最大数额，而不会出现政府明天想违约的可能性。假设未来信贷变得更加紧张——明天的债务上限下降。由于政府更难以平滑消费波动，其对获得信贷的感知收益现在较低，因此其偿还今天债务的意愿下降。作为回应，投资者也将今天的债务上限降低。

通过这个过程，宽松信贷和高偿还债务意愿的平衡可能转变为紧缩信贷和低偿还意愿的平衡。同样，在 1981 年 Eaton 和 Gersovitz 的完整模型中，存在风险债务，投资者对违约可能性的悲观预期可能转化为债务更高的风险溢价——这通过使债务服务成本更高和继续进入信贷市场更无价值，将鼓励违约并证实最初的悲观预期。这种机制听起来很有吸引力，在我们看来，它捕捉了主权债务市场均衡多重性的共同直觉的一个重要部分。

我们的研究结果排除了这种可能性。在Zhang (1997)的环境中，直觉仍然是最简单的。如果存在两个具有不同债务限额的均衡，我们考虑两个在各自均衡中都达到极限的政府。我们认为债务较少的政府必须具有严格更高的价值：从这一点开始，它可以遵循一种与债务较多的政府相似的策略，保持其负债在统一距离，并通过对利息支付进行节约，在每个点实现更高的消费。但这与假设两个政府都从其债务限额开始，每个政府都必须获得违约的（恒定）价值相矛盾。简而言之，一旦两个政府都耗尽了它们的债务能力，债务水平严格较低的政府就严格更好——这意味着该政府应该能够借更多的钱而不冒违约的风险，并且毕竟没有耗尽其能力。

## Model
We now describe what we call the _benchmark_ infinite-horizon model with Markov income (see [Aguiar and Amador, 2015](https://www.sciencedirect.com/science/article/pii/S0304393216301155?via=ihub#bib1)). We focus first on **Markov perfect equilibria**, in which the current states _b_ and _s_ encode all the relevant history. In [Section 2.3](https://www.sciencedirect.com/science/article/pii/S0304393216301155?via=ihub#s0025) we will show that this is without loss of generality, since one can specify this model as a game whose **only subgame perfect equilibria are Markov perfect equilibria.**

An exogenous state $s$ follows a discrete $\underline{\text{Markov chain}}$ with elements in $\mathscr{S}$, $|\mathscr{S}| = S \in \mathbb{N}$, and transition matrix $\pi\left(s' | s\right)$. Output $y\left(s\right)$ is a function of this underlying state.

At the beginning of each period, the government starts with some level of debt $b\in\mathscr{B}.$ After observing the realization of $s$, it decides whether to repay $b$ or default. If it does not repay, it receives an exogenous value $V^d(s)$, which encodes all the consequences of
default. **The assumption that $V^d(s)$ is exogenous and independent of $b$ follows some of the quantitative sovereign debt literature**. This assumption is important for the current result. When the literature has considered **endogenous $V^d(s)$,** it has typically been by **including a stochastic reentry option**; we will consider this possibility in Section 4.2.

If the government does not default, it receives $y(s)$ as endowment, pays $b$,and issues new
bonds $b^\prime\in\mathscr{B}$ that will be due next period, raising revenue $Q(b^\prime,s).$ Its (possibly state dependent) **flow utility** from consumption is $u(c,s)$, so that the value $V$ from repayment is given by

$$V(b,s)=\max_{b^{\prime}}u(c,s)+\beta\mathbb{E}_{s^{\prime}|s}\left[V^o(b^{\prime},s^{\prime})\right] \quad \mathrm{s.t.}\quad c+b=y\left(s\right)+Q(b^{\prime},s)$$
and the value $v^\mathrm{o}$ including the option to default at the beginning of a period is given by
$$V^o(b,s)=\max_{p\in\{0,1\}}pV(b,s)+(1-p)V^d(s)$$

where $p=1$ denotes the decision to repay and $p=0$ denotes the decision to default.

Debt is purchased by **risk-neutral** international investors that demand an expected return
of $R$. For convenience, we assume that when a government is indifferent between
repayment and default, **it chooses to repay**: $p(b,s)=1$ if and only if $V(b,s)\geq V^d(s)$
Since investors receive expected repayment $\mathbb{E}_{s^{\prime}|s}[p(b^{\prime},s^{\prime})]$, if follows that the **bond**
**revenue schedule $Q$** is
$$Q(b’,s)=\frac{b’}R\mathbb{E}_{s’|s}\left[p\left(b’,s’\right)\right]=\frac{b’}R\mathbb{P}_{s’|s}\left[V(b’,s’)\geq V^d(s’)\right]$$
where $\mathbb{P}_{s^{\prime}|s}\left[\cdot\right]$ is the conditional probability operator. We are now ready to define Markov
perfect equilibrium, which is the typical focus in the literature.

> Here implies that  $$ RQ(b',s)=  b' E[p]$$if we let $R$ be exogenous, then it's easy to define that $Q$ is indeed a function representing bond quantity that **international investors are willing to lend**


### Definition 1

A Markov perfect equilibrium is a set of policy functions $p(b,s),c(b,s),b^{\prime}(b,s)$ for
repayment, consumption and next period debt, value functions $V(b,s)$ and $V^o(b,s)$, and a bond revenue schedule $Q(b^{\prime},s)$, all defined on the set $\mathscr{B}\times\mathscr{S}$,such that (1),(2),(3) are satisfied.

We first prove an existence result-to our knowledge, the first such formal result in the
literature. For this we make the following four assumptions.

1. Assumption 1
	$\beta\in(0,1)$,and for each s,$u(\cdot,s)$ is continuous and strictly increasing
2. Assumption 2
	There exist $\gamma>0$ and $\kappa>0$ such that $u(c,s)\leq\gamma c^\kappa$ for all $c,s;$ and $\beta R^\kappa<1.$
3. Assumption 3
$$\lim_{c\to0}u\left(c,s\right)=-\infty.$$
4. Assumption 4
$$\mathscr{B}=\begin{bmatrix}\underline{b},\bar{b}\end{bmatrix},\mathrm{where~}-\infty\leq\underline{b}\leq0<\bar{b}<\infty.$$
> Assumption 4 means that the sovereign can issue debts and make savings.

Assumption 1 is a standard restriction on preferences. Assumption 2 guarantees that the
government cannot **obtain unboundedly high utility by deferring consumption**
**indefinitely and earning interest on the resulting savings**. Assumption 3 ensures that the
government is never at a corner of zero consumption, since such corner solutions can lead to analytically intractable discontinuities in $V.$ Assumption 2,Assumption 3 are jointly satisfied by some common parametric specifications, including CRRA utility $u\left(c,s\right)=\frac{c^{1-\sigma}-1}{1-\sigma}$ for any $\sigma\geq1.$
Assumption 4 includes several restrictions on allowable bond positions. 
The upper bound $\bar{b}<\infty$ rules out **Ponzi schemes**; it can be chosen high enough not to be binding. $\bar{b}>0$ restricts our focus to cases where debt is allowed. Our assumption that $\underline{b}\leq0$ allows the government to pay down all of its debt if it so desires, and possibly to save.For now,$\underline{b}$ is left otherwise **unrestricted**. We also need an assumption to guarantee that **default is never optimal when the government has positive assets.** Define $V^{nb}(b,s)$ to be the value function for a government that can **save at the risk-free rate but not borrow**,
$$V^{nb}(b,s)=\max_{b^{\prime}}u(c,s)+\beta\mathbb{E}_{s^{\prime}|s}\left[V^{nb}(b^{\prime},s^{\prime})\right]\mathrm{s.t.}\quad c+b=y\left(s\right)+\frac{b^{\prime}}{R},\:\underline{b}\leq b^{\prime}\leq0\quad(4)$$
Then we assume
5. Assumption 5
$$-\infty<V^d(s)\leq V^{nb}(0,s).$$
Assumption 5 is satisfied, for example, **if default is punished by permanent autarky, with**
**output also reduced exogenously**. In that case, $v^d$ is defined recursively by
$$V^d(s)=u(y(s)-\tau(s),s)+\beta\mathbb{E}_{s^{\prime}|s}\left[V^d(s’)\right]$$
for any exogenous cost of default $\tau(s)\in[0,y(s)].$



### 2.2. Uniqueness of Markov perfect equilibrium

Suppose that we have two distinct revenue schedules Q and $\widetilde{Q}$,each derived via (7) from
anticipated default thresholds $\left\{b^*(s)\right\}_{s\in\mathscr{S}}$ and $\left\{\tilde{b}^*(s)\right\}_{s\in\mathscr{S}}.$ Let $V$ and $\widetilde{V}$ be the value
functions for a government facing these schedules. To prove uniqueness of equilibrium we need to show that at most one of these value functions can be consistent with the default thresholds that generate it-in other words, that we cannot have both $V(b^*(s),s)=V^d(s)$ and $\widetilde{V}(\tilde{b}^*(s),s)=V^d(s)$ for all s.

**The key observation of this paper is that we can derive a simple inequality for the two**
**value functions$V$and $\widetilde{V}$,** related to the maximum difference between the default thresholds. This inequality requires Assumption 1,Assumption 2, Assumption 3, Assumption 4,Assumption 5 together with two crucial new assumptions:
6. Assumption 6
$$R>1.$$
7. Assumption 7
$$\underline{b}=-\infty.$$
The basis of our inequality is a simple replication strategy we call ***mimicking at a distance***
Suppose that $b^*(s)$ exceeds $\tilde{b}^*(s)$ by at most $M>0.$ Then we show that it is always
weakly better to start with debt of $b-M$ when facing prices $\widetilde{Q}$ than with debt of $b$ when
facing prices Q. and indeed strictly better whenever $V(b,s)\geq V^d(s).$ This observation, formalized in Lemma 1, will ultimately be the basis of the proof that distinct equilibria are impossible in Proposition 2.

### Lemma 1 Mimicking at a distance.

Let Q and $\widetilde{Q}$ be two distinct revenue schedules, with Q reflecting expected default thresholds $\left\{b^*(s)\right\}_{s\in\mathscr{S}}$ and $\widetilde Q$ reflecting expected default thresholds $\left\{\tilde{b}^*(s)\right\}_{s\in\mathscr{S}}.$ Let Vand $\widetilde{V}$ be the respective value functions for governments facing these revenue schedules. Define
(8)
$$M=\max_sb^*(s)-\tilde{b}^*(s)$$
and assume without loss of generality that $M>O.Then,for$ any s and b,
$$\widetilde{V}(b-M,s)\geq V(b,s)$$
(9)

with strict inequality whenever $V(b,s)\geq V^d\left(s\right).$

## Proof

First, note that for any $b$ 'and s, applying(7) we have

(10)
$$\begin{aligned}&\widetilde{Q}\left(b^{\prime}-M,s\right)=\frac{(b^{\prime}-M)}R\sum_{\left\{s^{\prime}:b^{\prime}-M\leq\tilde{b}^{*}(s^{\prime})\right\}}\pi\left(s^{\prime}|s\right)\geq\frac{(b^{\prime}-M)}R\sum_{\left\{s^{\prime}:b^{\prime}\leq b^{*}(s^{\prime})\right\}}\pi(s^{\prime}|s)\\&>\left(\frac{b^{\prime}}R\sum_{\{s^{\prime}:b^{\prime}\leq b^{*}(s^{\prime})\}}\pi(s^{\prime}|s)\right)-M=Q(b^{\prime},s)-M\end{aligned}$$
Thus the amount that a government with schedule $\widetilde{Q}$ can raise by issuing $b^{\prime}-M$ of debt is always strictly larger than the amount that a government with schedule Q can raise by issuing $b$ 'of debt, minus $M.$ The two intermediate inequalities in (10) reflect the two
sources of this advantage. First, there are weakly more cases in which $b^{\prime}-M\leq\tilde{b}^*(s^{\prime})$ than in which $b^{\prime}\leq b^*(s$ '), and this higher chance of repayment makes it possible to raise more. Second, since Assumption 6 requires $R>1$, issuing M less debt costs strictly less than M in foregone revenue in the current period.

This inequality leads us to consider the following **mimicking at a distance policy** for a government starting with debt $b-M$ and facing prices $\widetilde{Q}.$ This government has the option to mimic the policy of the government with debt $b$ facing prices $Q$ -always
defaulting at the same points, and otherwise choosing the same level of debt for the next period minus $M.$ Such mimicking is possible, irrespective of the value of $M>0$,**because savings is unrestricted (Assumption 7)**. Due to inequality (10), the former government
will achieve strictly higher consumption than the latter government in every period prior
to default, and therefore a strictly higher value overall.

More formally, for any states and debt levels s and $b$,let the history s$^{0}$be such that the
state and debt owed at $t=0$ are respectively s and $b.$ The optimal strategy for a
government facing schedule Q induces an allocation $\left\{c\left(s^{t}\right),b\left(s^{t-1}\right),p\left(s^{t}\right)\right\}s^{t}\succcurlyeq s_{0}$ at all histories following s$^{0}$ We construct a policy for the government facing schedule $\widetilde{Q}$ in state s and debt level $b-M$ as follows. For every history $s^\mathrm{t}$ following and including s$^{0}$,let
$$\tilde{p}\left(s^t\right)=p\left(s^t\right)$$
and provided that $p\left(s^t\right)=1$,choose consumption and next-period debt as
$$\tilde{b}\left(s^t\right)=b\left(s^t\right)-M\tilde{c}\left(s^t\right)=c\left(s^t\right)+\widetilde{Q}\left(b\left(s^t\right)-M,s_t\right)-\left(Q\left(b\left(s^t\right),s_t\right)-M\right)$$
Note that $\tilde{b}\left(s^t\right)\in\mathscr{B}$ due to Assumption 7. This choice of $\tilde{b}$ and $\tilde{c}$ ensures that the budget
constraint is satisfied at all histories $s^{t}$ where repayment takes place:
$$\begin{aligned}&\tilde{c}\left(s^t\right)+\tilde{b}\left(s^{t-1}\right)-\tilde{Q}\left(\tilde{b}\left(s^t\right),s_t\right)=\tilde{c}\left(s^t\right)+b\left(s^{t-1}\right)-M-\widetilde{Q}\left(b\left(s^t\right)-M,s_t\right)\\&=c\left(s^t\right)+b\left(s^{t-1}\right)-Q\left(b\left(s^t\right),s_t\right)=y\left(s_t\right)\end{aligned}$$
> if you're confused later on, just know that $\tilde{c}$ comes from the same budget constraint

Furthermore, using(10) we see that $\tilde{c}(s^t)>c(s^t)$: when there is repayment, the
mimicking policy (11) sets consumption $\tilde{c}(s^t)$ equal to consumption $c(s^t)$ in the other equilibrium, plus a **bonus** $\widetilde{Q}\left(b\left(s^t\right)-M,s_t\right)-\left(Q\left(b\left(s^t\right),s_t\right)-M\right)>0$ from **lower debt costs**.

The mimicking policy, of course, need not be optimal; **but since it is feasible, it serves as a lower bound for $\widetilde{V}(b-M,s){:}$**
$$\begin{aligned}&\widetilde{V}\left(b-M,s\right)\geq\sum_{\tilde{p}\left(s^t\right)=1}\beta^t\Pi\left(s^t\right)u\left(\tilde{c}\left(s^t\right),s_t\right)+\sum_{\tilde{p}\left(s^t\right)=0,\tilde{p}\left(s^{t-1}\right)=1}\beta^t\Pi\left(s^t\right)V^d(s_t)\geq\\&\sum_{p(s^t)=1}\beta^t\Pi\left(s^t\right)u\left(c\left(s^t\right),s_t\right)+\sum_{p(s^t)=0,p\left(s^{t-1}\right)=1}\beta^t\Pi\left(s^t\right)V^d(s_t)=V(b,s)\end{aligned}$$
with strict inequality whenever $p(s^0)=1\left(\text{or equivalently }b\leq b^*(s)\right)$, since this implies
$\tilde{c}(s^0)>c(s^0)$ and $u\left(c,s_0\right)$ is strictly increasing in $c$ thanks to Assumption 1.

> here $\Pi(s_t)$ should be the stationary distribution probability of $s_t$ 

An illustration of the mimicking policy used in Lemma 1 is given in Fig. 1a and b, which depict time paths in a hypothetical two-state case. In this case, debt starts relatively high and the high-income state $y\left(s_H\right)$ keeps recurring, leading the government to deleverage in anticipation of lower incomes in the future. Fig. 1a shows the paths of $b$ (filled circles) and the mimicking policy $\tilde{b}=b-M$ (hollow circles), while Fig. 1b shows the paths of $c$ (filled circles) and the consumption $\tilde{c}=c+\widetilde{Q}(b-M,s)-(Q(b,s)-M)$ induced by the mimicking policy (hollow circles). Observe that $\tilde{c}$ is always greater than $c.$
![[Pasted image 20240808174228.png]]

Fig. 1.(a) Example paths for$b$and$\tilde{b}$ and (b) example paths for $c$ and $\tilde{c}.Notes:$ Illustration of the mimicking policy used in Lemma 2. The filled circles represent the original policy $(b,c)$,and the hollow circles the mimicking policy $(\tilde{b},\tilde{c}).1$a shows that the debt of the mimicking government $\tilde{b}$ is always at a constant distance M below $b.1$b shows that
consumption of the mimicking government $\tilde{c}$ is always strictly above $c.$ However, the gap
$\tilde{c}-c$ differs across periods. This reflects **fluctuations in the two sources of** $\tilde{c}-c:$
differences in **default premia**, and the lower cost of servicing $\tilde{b}=b-M$ rather than $b.$ 

First, since both debt levels at $t=2$ are above the respective default thresholds for $y(s_L)$, there is no difference at $t=1$ in the two default premia. At $t=3$, however, **the mimicking policy achieves a debt level below $\tilde{b}^*(s_L)$,** while the other policy has debt that remains above $b^*(s_L).$ Thus the **default premium disappears at $t=2$ for the mimicking policy** while
still being paid for the other policy, l**eading to an expansion in the gap** $\tilde{c}-c.$ From $t=4$
onward both policies achieve debt levels below their s$_L$ default thresholds, **leading to the disappearance of all default premia.** This causes the gap $\tilde{c}-c$ to compress starting at $t=3.$ 

