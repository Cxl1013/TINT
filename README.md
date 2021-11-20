
# 机组数据驱动的风电场短期风况预测


```python
比赛地址: https://www.industrial-bigdata.com/
```

# 运行环境


```python
python3.6
dtw==1.4.0
dtw_python==1.1.8
Keras==2.4.3
lightgbm==2.3.1
matplotlib==2.2.2
numpy==1.21.4
pandas==1.1.5
scikit_learn==1.0.1
scipy==1.2.0
tensorflow_gpu==2.4.0
tqdm==4.32.1
tsmoothie==1.0.4
```

# 模型描述


```python
初赛:
    LGB:包含特征递归的LGB模型
    DTW:基于子序列相似性的时序预测
    seq2seq:基于LSTM的seq2seq模型
决赛:
    仅使用了seq2seq模型
```

# 程序运行说明


```python
KalmanSmoother.ipynb  合并提供的数据，每个风机生成一个文件（包含对风速使用卡尔曼滤波）
DWT.ipynb  基于DWT的预测模型(未对测试集进行预测)
LGB.ipynb  基于LGB的预测模型(未对测试集进行预测)
seq2seq_dir.ipynb  基于LSTM的seq2seq模型(风向预测)
seq2seq_spd.ipynb  基于LSTM的seq2seq模型(风速预测)
predict.ipynb  决赛预测(seq2seq)
```
