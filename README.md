# uda_neural_network_bicycle


| Command | Description |
| --- | --- |
| `git status` | List all *new or modified* files |
| `git diff` | Show file differences that **haven't been** staged |


> 运行结果记录


| epochs| lr  | outputnodes | hiddenodes | Trainingloss | Validationloss |
| ---   | --- | --- | --- | ---   | --- | ---|
| 3500  | 0.5 | 1   | 6  | 0.081 | 0.168 |
| 10000 | 0.5 | 1   | 7  | 0.055 | 0.152 |
| 10000 | 0.5 | 1   | 8  | 0.055 | 0.130 |
| 10000 | 0.5 | 1   | 9  | 0.060 | 0.186 |
| 10000 | 0.5 | 1   | 10 | 0.062 | 0.198 |

hiddennode 到达8个的时候，过拟合严重

发现其实迭代到3000多就到底了 - -

感觉在6的时候最好

> 遗留问题

1. 从12月22日开始，prediction和data之间的差值明显上升了，猜测是出现其他的因素造成数据比predication要低。
2. 如何确定此时是否是局部最低点？
3. 如何加入dropout，还有正则化？
4. 迭代次数一多，每次运行都会很慢。 - - 

