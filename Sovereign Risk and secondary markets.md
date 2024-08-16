
**例3. (幸运-不幸世界)**: 这个世界持续两个时期：今天和明天，用\(t \in \{0,1\}\)表示，它包含两个等大小的区域：家和外国，用\(j \in \{H,F\}\)表示。每个区域包含\(a\)个连续的无限小个体，它们最大化熟悉的效用函数：\(U(c_{i0}, c_{i1}) = u(c_{i0}) + u(c_{i1}) \)，对所有\(i \in \mathcal{I}^W = \mathcal{I}^H \cup \mathcal{I}^F\)。所有个体今天都收到一份$y$的禀赋。但明天有两种状态。如果\(s = s^H\)，家是幸运的，其居民收到等于\(y + \varepsilon\)的禀赋，而"外国是不幸的，其居民"收到等于\(y - \varepsilon\)的禀赋。如果\(s = s^F\)，家是不幸的，其居民收到等于\(y - \varepsilon\)的禀赋，而"外国是幸运的，其居民收到等于\(y + \varepsilon\)的禀赋。两种状态发生的概率相等。

显然，在幸运-不幸世界（L-U世界）中，通过国际风险共担可以获得收益。通过汇集他们的禀赋，个体可以在不牺牲平均消费水平的情况下消除消费的波动性。但我们将考虑一种情况，即保险市场缺失。唯一可交易的资产是一种非条件性债券。在完全执行的情况下，没有国际贸易，每个区域都被迫消费自己的禀赋。如果预期是乐观的，那么在战略执行下也会发生同样的情况。这一结果不是帕累托有效的，当然，原因是市场不完整。

但还有另一种均衡，它结合了乐观和悲观的预期，可以提高所有人的福利并实现帕累托效率。假设个体预期幸运区域的居民会强制执行彼此之间的债券支付，而不幸区域则不会这样做。鉴于这些预期，存在一种交易策略，确保完全的风险共担：在一级市场上，每个个体购买由另一区域居民发行的 $ε$ 债券，并通过发行和销售$ε$ 债券来为这次销售融资。如果一个个体最终是不幸的，他/她将违约，并享受等于$y$的消费。如果一个个体最终是幸运的，他/她将遭受等于ε的资本损失，并同样享受等于$y$的消费。

发生了什么？悲观情绪关闭了市场（如Dupond债券市场）和/或导致均衡违约（如当一个区域最终是不幸时）。在D-C世界中，市场是完整的，因此，完全执行的分配是帕累托有效的。在这个最优环境中，关闭市场和/或引发违约总是减少了福利。在L-U世界中，保险市场缺失，完全执行的分配不再是帕累托有效的。在这个次优环境中，众所周知，关闭一些市场和/或使用违约来改变现有资产的范围可能会导致帕累托更优的结果。这种经典的次优直觉解释了为什么悲观的预期有时可能比乐观的预期带来更高的福利。

到目前为止，我们已经展示了以下几点：（i）总存在一个乐观的均衡状态，它提供的消费者水平和福利与完全执行均衡状态下的相同；（ii）还有一些具有战略性执行的额外均衡状态，这些状态以对执行的悲观预期为特征，并涉及不同水平的消费和福利；（iii）乐观均衡状态不一定是提供最高可能福利的那个。我们接下来要讨论的主题是稳健性。

### Robustness

为了评估具有战略性执行的均衡的稳健性，我们假设政府每次决定不执行支付时都会遭受相当于 \( b \) 的小福利损失。我们将 \( b \) 视为任意小但严格为正的数。特别是，在债务-债权世界（D-C World）中，这意味着债务国政府的目标函数现在由 \( W^D = \int_{i \in \mathcal{I}^D} u(c_{i1}) - b (2 - e_C^D - e_D^D) \) 给出。我们环境中的这个小修改消除了所有基于悲观预期的均衡，因此，乐观均衡是唯一稳健的。

这个结果背后的原因相当简单。如果个体预期债务国政府明天不执行任何债券支付，那么今天不会有债务国发行的债券被交易。在没有执行偏好的情况下，即 \( b=0 \)，这意味着政府对执行和不执行持中立态度，后者因此是最佳响应。有小的执行偏好，即 \( b>0 \)，情况就不再是这样：**每当执行决定对消费或福利没有影响时，政府将选择事后执行支付，因此不执行在均衡中就不可能发生。**

因此，我们给结果列表增加了第四项，也是最后一项：（iv）只有乐观均衡在引入（任意小的）执行偏好时存活下来。这使我们选择债务-债权世界中的乐观均衡。然后我们将这个均衡与完全执行均衡之间的差异称为主权风险的影响。**我们的主要结果是，如果个体可以自由重新交易现有资产，主权风险对消费和福利没有影响。** 主权风险的唯一影响是增加交易量，因为个体不仅为了平滑消费而交易，也为了规避政府的战略性或机会主义行为。

### Commitment and Enforcement

我们在本节结束时提醒读者注意一个微妙但重要的问题。到目前为止，我们已经展示了次级市场能够在政府没有承诺并选择战略性执行时，恢复完全执行的分配。**这种情况在 time inconsistency 文献中通常被称为“自由裁量discretion”**。一些读者可能已经想知道，为什么我们没有使用更常见的术语来指代一个政府有 commitment 的经济体，而不是指一个full enforcement 的经济体。这两种选择在根本上难道不是一样的吗？在本节中，我们将解释为什么它们不是。

普遍认为承诺导致完全执行的观点，我们认为，是基于具有完全市场和代表性代理人的模型的普遍性。当市场不完全时，承诺通常不会导致完全执行。例如，考虑例3中的L-U世界，在这个世界中，每个区域包含一个代表性个体，但由于缺乏contigent bonds，市场是不完全的。正如我们在D节中论证的，在这个世界中，完全执行的分配是无效率的。**实际上，full enforcement 使可用资产变得无用**。如果家和外国有承诺，他们今天会同意以下执行政策：幸运区域执行所有债券支付，而不幸区域执行“无”。这种执行模式将增加非条件性债券的范围，并导致世界上所有个体的预期效用更高。因此，在这个世界中，commitment 将通过防止次级市场导致完全执行的分配来提高福利。**This is therefore a world in which discretion delivers the allocation with full enforcement, but commitment does not.**

当代理人是异质的时候，承诺也未必导致完全执行。例如，考虑例2中的D-C世界，但假设债务国政府只关心杜邦人，即 \( W^D = \int_{i \in \mathcal{I}^D} \phi_i u(c_{i1}) \) 其中 \( \phi_i = 1 \) 如果i是Dupont，而 \( \phi_i \approx 0 \) 如果i是Dupond。在这个世界中，市场是完全的，但债务国内部存在异质性。
If Debtor’s government had commitment, it would choose to enforce bond payments by Duponts and not to enforce bond payments by Duponds. This would effectively remove Duponds from the primary market, lowering the supply of bonds and improving the terms at which Duponts borrow. This enforcement policy would raise the welfare of Duponts and that of Debtor’s government at the expense of Duponds (and creditors). As in the previous case, commitment does not lead to the full-enforcement allocation.

到目前为止的所有例子中，政府更倾向于事后不执行支付。我们刚刚看到了两个例子，政府也倾向于事先不执行一些支付。在这些情况下，承诺均衡与完全执行均衡有不同的消费和福利。后者可以通过战略性执行和次级市场实现，但前者不能。

## The General Case
结果（i）至（iv）是通过一种非常程式化的设定帮助得出的。这有助于建立直觉。但这些结果适用于一个非常广泛的模型类别，包括许多在以往文献中使用的模型。在这一部分，我们在具有多个区域、多个时期、多次冲击、多种市场不完全性和区域内外多种异质性来源的一般设定中，提供了这些结果的正式证明。
由于显而易见的原因，本节的风格比前一节更为正式和技术性。一些读者可能更愿意首先阅读第三节，在那里我们回到第一节的非正式风格，并使用D-C世界的简单变体来展示论证的局限性并进一步发展直觉。

### Model

考虑一个包含$J$个区域的世界经济体，区域由$j\in\mathcal{J}\equiv\{1,2,...,J\}$索引。每个区域包含一系列无限小的个体。我们用$\mathcal{I}^j$表示位于区域$j$的个体集合，而$\mathcal{I}^W=\cup_{j\in\mathcal{J}}\mathcal{I}^j$表示全世界的总人口。设$j(i)$表示个体$i$所在的区域，即如果$i\in{\mathcal{I}}^{j'}$，则$j(i)=j'$。

这个世界持续$T+1\leq\infty$个时期，由$t\in\mathcal{T}\equiv\{0,1,...,T\}$索引。在每个时期$t$内，时间顺序如下：(i) 实现冲击$s_t\in S$，个体获得  *perishable consumption good* 的禀赋$y_{is_t}\geq0$，(ii) 资产市场开放，个体重新交易现有资产并发行新的资产，(iii) 政府决定对到期资产的执行，(iv) 执行发生，以及 (v) 个体消费。


$\operatorname{Let}s^t\equiv(s_\tau|\tau=0,1,...,t)\in{\mathcal{S}^t}$ denote the history of realizations of the shock up to period $t.$ Let $\mathbf{e}_t$ and $\mathbf{x}_t$ denote, respectively, the profile of enforcement choices of all governments and the profile of post-trade asset holdings of all individuals in period $t.$ Let $h^t\equiv(s_\tau,\mathbf{e}_\tau,\mathbf{x}_\tau|\tau=0,1,...,t)$ $\in\mathcal{H}^t$ denote the history of shocks and actions by governments and individuals up to period $t$, $h^{0t}\equiv(h^{t-1},s_t)\in\mathcal{H}^{0t}$ denote the history of shocks and past actions by governments and individuals up to period $t$, and $h^{1t}\equiv(h^{0t},x_t)\in\mathcal{H}^{1t}$ denote the history of shocks, actions by individuals, and past actions by governments up to period $t.$ The probability of observing a history $h^\tau$,conditional on having observed a history ${h^{0t}}$, is denoted $\pi(h^\tau|h^{0t}).$ Let $\mathcal{S}\equiv\cup_{t\in T}S^t,\mathcal{H}\equiv\cup_{t\in T}\mathcal{H}^t$, $\mathcal{H}^0\equiv\cup_{t\in T}\mathcal{H}^{0t}$, and $\mathcal{H}^1\equiv\cup_{t\in T}\mathcal{H}^{1t}.$

