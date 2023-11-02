# FastDiff语音合成任务

数据集：LJSpeech  
LJSpeech由13100个22050赫兹的音频片段组成，女性，总共约24小时。  
数据集：VCTK  
由大约44200个音频片段组成，这些音频片段由109名以英语为母语的不同口音的人发出。  

VCTK数据集被下采样到22050 Hz，以将采样率与LJSpeech数据集相匹配。  
FFT大小、窗口大小和跳变大小分别设置为1024、1024和256。  
特征选择：80波段Mel频谱图
>Mel频谱图 (Mel Spectrogram): Mel频谱图是一种频谱图，用于表示声音信号的频率内容。它将声音信号分成一系列短时间窗口，每个窗口内的声音信号被认为是稳定的。然后，对每个窗口应用傅立叶变换，将声音信号从时域转换为频域。80波段 (80 Bands): Mel频谱图通常被分成多个频带，通常称为"波段"。这些波段是频率范围的分段，用来表示声音信号中不同频率范围的能量。"80波段"表示将频谱分成80个这样的频率范围。
>
训练环境：4个NVIDIA V100 GPU  
评价指标：MOS分数、STOI和PESQ  
![image](https://github.com/zhangwenjingustb/TTS/assets/141011729/ed487647-2e00-4886-9cb6-51dcb5301f60)  
缺点：多样性方面比不上wavenet  

# MockingBird
https://github.com/babysor/MockingBird  
自己电脑

# 论文合集
https://github.com/zzw922cn/awesome-speech-recognition-speech-synthesis-papers  





