# Phonetics and Synthesis

Almost a Chinese translation of [Modern speech synthesis for phonetic sciences](https://people.kth.se/~ghe/pubs/present/malisz2019modern-slides.pdf), assisted by ChatGPT 4o.

## Take-home message

- 语音技术（speech technology）和语音科学（speech sciences）曾经对话互利
  
  - 注：Speech Science 与 Phonetics 似乎并不能画等号。参见 [PALS0009 Introduction to Speech Science](https://www.phon.ucl.ac.uk/courses/pals0009/week1.php)，[Sprechwissenschaft und Phonetik/ Speech Science and Phonetics](https://www.uni-marburg.de/en/studying/degree-programs/humanities/m-speechscience-phonetics)，[Speech Science - The University of Auckland](https://www.auckland.ac.nz/en/study/study-options/find-a-study-option/speech-science.html) 以及 [Speech science - Wikipedia](https://en.wikipedia.org/wiki/Speech_science)。德语中有 [Sprechwissenschaft](https://de.m.wikipedia.org/wiki/Sprechwissenschaft) 和 [Sprachwissenschaft (Linguistik)](https://de.m.wikipedia.org/wiki/Sprachwissenschaft) 之分，待考。另外，我们注意到 speech/parole 在索绪尔用法中的“言语”含义。

- 优先事项不同，分道扬镳

- 近来合成的进展消除了语音科学家旧的障碍

- 两个领域的兴趣正在趋同

- 技术人员和科研人员共同的机会

## 两个领域

### 语音合成 -> 语音学

- 语音范畴化感知（Categorical speech perception）：合成声音连续统（synthetic sound continua）(Lisker and Abramson, 1970)

- 语音感知的肌动理论（Motor theory）(Liberman and Mattingly, 1985)、[声学线索（acoustic cue）](https://www.oxfordreference.com/display/10.1093/oi/authority.20110803095347862)分析

- 用合成来分析：用以测试病理模型的建模框架 (Xu and Prom-On, 2014; Cernak et al., 2017)

### 语音科学 -> 合成

- 在数据稀疏、共振峰合成时代，语音科学对语音处理和工程大有裨益 (King, 2015)

- Phones and phone sets

- 基于感知的建模，如 mel scale (Stevens et al., 1937)

- 源自心理语言学的复杂的语音合成评价方法 (Winters and Pisoni, 2004; Govender and King, 2018)

### 为什么技术人员需要语音科学？

- 合成和分析携手并进

- 为了理解数据和结果（不只是描述）

- 为了严谨的评估和分析途径

### 为什么语音学家需要语音合成？

- 生成刺激（Stimulus creation）：单独评价听者对特定声学线索的敏感度
  
  - 操纵诸如共振峰过渡等因素，同时排除多余和残留的发音部位线索
  
  - 控制单一线索的变化，限制混淆因素（confounds）
  
  - PSOLA, MBROLA, STRAIGHT 以创建、操纵语音 (Moulines and Charpentier, 1990; Dutoit et al., 1996; Kawahara, 2006)
  
  - 语音失真（distortion）和 delexicalisation；noise-vocoding (White et al., 2015; Kolly and Dellwo, 2014)

## 为什么合成语音在当代语音科学如此少见？

- 较新的语音合成无法提供语音学研究所需的精确控制

- 社区之间的重叠很少，意味着少有语音学家具备技术知识，以将合成的发展适用于其需求

- 自然语音和经典合成语音之间的感知差异，对研究结果的普遍性提出了质疑

### 近期（2019年以前）语音合成自然度的成果

- 使用神经声码器（neural vocoders），如 WaveNet (van den Oord et al., 2016)，生成高度自然的语音信号
- 通过端到端（end-to-end）方法，如 Tacotron (Wang et al., 2017)，极大地改善了 TTS （在英语中）的韵律
- 在 MOS 中，TTS 的自然度接近录制的语音 (Shen et al., 2018)

### 感知问题

根据 Winters 和 Pisoni（2004）的综述，一系列研究表明，经典的共振峰合成：

- 比录制的语音可懂度低

- 过度占用注意力和认知机制，导致处理时间变慢 (Duffy and Pisoni, 1992)
  
  此外，自然度评分也很低

## 我们相信

- 技术人员应当追求现代语音合成范式的精准输出控制

- 科研人员应关注并为这些发展做出贡献

- 感知不足的问题已基本得到解决

### 语音合成的过去、现在、将来 🚀✨🌌

![Past and Future.png](./img/Then_and_Now.png)

### 新的技术研究示例

- 用于语音学的可控神经声码器：将 MFCC 控制界面 (Juvela et al., 2018) 替换为更具语音学意义的语音参数
  - 这些语音参数也可以从文本中预测，例如使用Tacotron
- 控制高层语音特征，例如显著性（prominence）(Malisz et al., 2017)

### 新的语音学研究领域示例

- 改进且可控的合成，不仅为既定的研究方向提供了更好的刺激，还开启了新的领域，例如：
  - “按需”生成会话现象（conversational phenomena）(Székely et al., 2019)
  - 生成难以从人类说话者中引出（elicit）的可选或非故意现象（例如，会话中的咔哒声）
  - “人工语音”与现实说话者的喋喋不休（babble），例如来自 unconditional WaveNet

### 新的联合研究（joint research）示例

- 针对当今功能强大的语音合成器的新型稳健且有意义的评估方法
- 结果：重燃语音科学和技术之间富有成效的对话

### 感知问题呢？

- 我们以前知道，经典的语音合成：
  - 自然度评分低于录制的语音
  - 可懂度低于录制的语音
  - 认知处理时间比录制的语音慢
- 这些问题在多大程度上仍然存在？
- 实证研究：比较自然语音、经典合成和现代深度学习合成在以下方面的表现：
  - 主观听众评分
  - 可懂度
  - 处理速度

使用开放代码和数据库以及适度的计算资源进行研究

## 总结与未来工作

- 能精确控制的现代语音合成，对科研人员和技术人员都很有吸引力
  
  - 这可以使这两个领域重新接触

- 现代合成语音在很大程度上克服了语音科学常用系统的感知不足
  
  - 操纵语音的情况需要进一步研究
  
  - 神经声码器、更多数据或更好的适应性，应该会进一步提高技术能力

- 让我们共同努力实现这一目标！

## TTS: A Unifying View

![A Unifying View.png](./img/Unifying_View.png)
