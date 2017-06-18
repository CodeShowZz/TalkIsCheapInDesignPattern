# TalkIsCheapInDesignPattern
## Talk is cheap,show me the code.

## 为什么建这个仓库
 看过大话设计模式,看过Head First设计模式,也有一本GOF.但是对我来说我看不下去Head First设计模式和大话设计模式了,可能由于大脑抗拒吧,而且GOF对我来说也可能有点深奥了,给出一些源码例子和一个基本的定义能让我迅速知道某个设计模式的最终意思。所以我决定从代码层面上学习设计模式。该仓库的代码会详细的举出一些例子来说明某种设计模式,并且会强调"演变"过程,通过使用后缀versionXX来指明,在代码中写入非常多个注释,以代码+注释的方式阐述一个模式。当然举出例子可能由于个人水平有所欠缺,但本仓库会不断改进。

## 个人观点
GOF这本书被誉为设计模式的鼻祖,但很多人看来这本书有点难以理解,其实这本书中带有很强的主观感受,比如作者举的一些例子,我们没有见过就感觉陌生,加上作者以一种非常高层次的行文风格,导致这本书确实很难理解。但是模式何止23种呢,模式的起源不就是很多人写的代码中的优秀套路集锦吗？个人认为设计模式在关注它的高层定义的同时,应该深入到具体的例子当中,比如书中说代理模式的应用十分广泛,说了一大堆,但是不给你一个比较直接的代码实例,你可能就不知道怎么用了。说白了,学设计模式是为了更好的写代码。如果有人反驳说代码没那么重要,还是研究类与类之间的关系,把定义背的滚瓜烂熟了,就能很好的运用了,那就是个人的口味问题了。觉得Git创始人Linux说的那句话挺对的(毕竟我写的东西是靠它上传的):**Talk is cheap,Show me the code.**。 举个例子来说吧,假如我要学代理模式,我应该从"代理"这两个字出发,先想想代理大致是什么意思.很简单吧.当然这样还不足以知道这个设计模式的真实意思,这个时候可以去找一些关于将"代理"的优秀的代码看一看,从简单到复杂,我想如果能理解优秀的例子了,这个时候让你向别人解释代理是什么意思时你就很自信了,而且你都会写代码了,类图肯定也能画得出来,反而有可能是一开始给你一个类图和一串定义让你觉得这东西太难。

## 模式并非标准
模式只是一些前辈们使用得很多的套路,并不是一个标准,没有人让我们写代码的时候处处见模式,而是当我们觉得我们的代码太冗余,太恶心的时候.恰当的使用几个模式进去。

## 模式详情(按照个人觉得简单到难的顺序排列）
 - TOP1 单例模式
 ### 标准定义
 > 保证一个类只有一个实例,并且提供一个访问它的全局访问点.
 ### 模式关键点
 - 私有化构造器
 - 定义一个静态的方法来实例化对象,但必须判断是否之前存在该对象,并且类中的引用也只能是静态的
 - 有预先生成实例或者延迟生成实例两种方式
 - 在多线程环境如果不加以控制,可能会出现多实例问题.
 
 - TOP2 策略模式
 
  ### 标准定义
 >  定义算法家族,封装每一个,使得它们可以替换,使得用户可以很独立的使用它们。 
 
 ### 模式关键点
 - 找出变化的和不会变化的方法,把会变的方法隔离出来
 
### 仓库中的代码
代码会以非常直观明了的方式来给出一个模式,当然这和个人的经验有关,当我发现一个更能体现某种模式的例子,我将毫不犹豫的写到这个仓库中来.
**代码周围有很多注释,建议代码一定要看懂,那些注释只是在语境下的一种补充,相互结合效果最佳!**

### DEBUG
有的设计模式比较简单,很容易理解.有的设计模式就比较独特,一时间难以捕捉其奥妙,所以需要DEBUG跟踪一下到底如何变化的,可以加深印象。

### 更多的模式
这本书提供的源码已经算不错了,但未能包括经典的23种模式源码,但模式远远不止23种,所以在未来希望提供更多的"模式"代码,但我想"模式"也不能全信,让时间去验证代码是否成功才是硬道理吧。

### 简单粗暴的补充资料
如果代码看懂了,却没有留下一个大体的轮廓在脑海中,那么这个时候就可以看看标准定义和类图了,下面的两个网站,可以找到相关的资料,或者尝试Google搜索某个模式,相信会有一大堆的图让你看

## http://sourcemaking.com 
## 维基百科  https://en.m.wikipedia.org/wiki/Software_design_pattern

### 自勉
与其陷入各种模式的禁锢之中,不如随机应变.
