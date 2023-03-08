# Music-Emotion-Classification
Input: 4-seconds music (sample rate: 22050Hz)

Output: One quadrant of Self-Assessment Manikin
> Q1: Happy (high valence, high arousal)
> 
> Q2: Tensional (low valence, high arousal)
> 
> Q3: Sad (low valence, low arousal)
> 
> Q4: Peaceful (high valence, low arousal)

<img src=https://upload.wikimedia.org/wikipedia/commons/6/6c/Valence-Arousal_Circumplex.jpg width=30% />

## Dataset
[Music-emotion](https://github.com/IanChen5273/Music-emotion/tree/main/music-emotion/song)

[turkish-music-emotion-dataset](https://www.kaggle.com/datasets/blaler/turkish-music-emotion-dataset)

<img src=./demo/1.png width=30% />

Total data:450(Music-emotion)+1000(Turkish)=1450

## Method 1: Machine Learning
### Feature Extraction
    - feature_mfcc (梅爾頻率倒譜係數) -> output 5 features
    - feature_rolloff (滾邊頻率) -> output 5 features
    - feature_spectral_contrast (頻譜對比) -> output 10 features
    - feature_rms (平方平均數) -> output 5 features

    25 features in every songs

### Select Machine Learning Model
<img src=./demo/2.png width=60% />
<img src=./demo/3.png width=60% />

## Method 2: CNN
### Model Structure
<img src=./demo/4.png width=60% />

### Result
<img src=./demo/圖片5.png width=60% />
<img src=./demo/圖片6.png width=30% />
<img src=./demo/圖片7.png width=30% />
