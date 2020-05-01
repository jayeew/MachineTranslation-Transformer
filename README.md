# 中文到英文的机器翻译
此模型完全基于[keras-transformer](https://github.com/CyberZHG/keras-transformer)，只是把别人的封装拿来简单实践一下<br>
此外，可以和我另一个基于LSTM的机器翻译项目[MachineTranslation-LSTM](https://github.com/jiayiwang5/MachineTranslation-LSTM)对比学习，二者原始数据一致
## 环境配置
| 程序         | 版本      |
| ---------- | ------- |
| python     | 3.68    |
| tensorflow | 1.13.1  |
| Keras      | 2.2.4   |
| windows10  |         |
| jupyter    |         |
## 实际效果
(注：中文正常输入无需空格)
| 输入中文 |输出英文  |
| :------------: |:---------------:|
| 我喜欢你！      | I like you ! |
| 你喜欢我吗？      |  Do you like me ?       |
| 滚蛋！  |  ***听不懂呢。***      |

(注：数据量较小可能遇到词典中没有的词，我简单的采用安全回复“听不懂呢。”来应对)
## 运行
### 方式一：完整过程
- **数据预处理**<br>
  `get_data`<br>
- **模型训练与预测**<br>
  `train&translate`<br>
### 方式二：加载现有模型
- 运行`train&translate`<br>
- 加载`model/W-- 40-0.0563-.h5` 
