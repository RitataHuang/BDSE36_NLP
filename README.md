# BDSE36_NLP -- 模型微調練習
## 中文句子情緒分類

## 訓練資料來源
- [Datasets:Johnson8187/Chinese_Multi-Emotion_Dialogue_Dataset](https://huggingface.co/datasets/Johnson8187/Chinese_Multi-Emotion_Dialogue_Dataset)

## 基礎模型
- [google-bert/bert-base-chinese](https://huggingface.co/google-bert/bert-base-chinese)

## 安裝套件
```
torch 版本: 2.6.0
torchvision 版本: 0.21.0
torchaudio 版本: 2.6.0
transformers 版本: 4.49.0
datasets 版本: 3.3.1
evaluate 版本: 0.4.3
accelerate 版本: 1.4.0
scikit-learn 版本: 1.6.1
importlib.metadata 版本: 8.5.0
```

## 說明
- 以google-bert/bert-base-chinese預訓練模型為基準微調，使用模型進行情緒分類，分成8類情緒。
```
    "平淡語氣": 0,
    "關切語調": 1,
    "開心語調": 2,
    "憤怒語調": 3,
    "悲傷語調": 4,
    "疑問語調": 5,
    "驚奇語調": 6,
    "厭惡語調": 7
```

- 預測以下文字，並且輸出預測的結果，以及 score (confidence，取得小數點後面第 2 位):
```
  texts = [
	"我每天都能跟她一起上學，我好開心！",
	"最好的朋友要離開臺灣了，以後可能不容易再見面...",
	"我覺得我快不行了...",
	"剛剛收到研究所錄取的通知書！",
	"今年的冬天好像比較晚來。"
	]
```

## 成果
- Youtube
https://youtu.be/m-sdWJOnlPU

- Result
<img width="461" alt="image" src="https://github.com/user-attachments/assets/3ace4619-2a17-4b14-a8bb-4f425de4d6f8" />

