# Kaggle Competition - Petfinder
---


# Team name/members
- **Team name :** shakeup is coming
- **Members**
  - [Park Hyunyong](https://github.com/hyunyongPark)
  - [Shin younghoon](https://github.com/Yphy)

<br/><br/><br/>
# Introduction
![image](https://github.com/hyunyongPark/Kaggle_petfinder/blob/main/imgs/competition_banner.PNG)

Kaggle 주최인 [Image Regression](https://www.kaggle.com/c/petfinder-pawpularity-score/overview)로서, 애완이미지(개, 고양이)의 이미지들과 여러가지 포즈나, 사진구도, 표정 등의 메타정보를 활용하여 Pawpularity(인기도)를 예측하는 task이다. 

<br/><br/><br/>
# Dataset / Evaluation

### 1) Dataset
![image](https://github.com/hyunyongPark/Kaggle_petfinder/blob/main/imgs/dataset_example1.PNG)

본 데이터셋은 위의 그림과 같이 각 이미지에 대한 인기도를 예측해야하며, 개,고양이에 대한 이미지 파일들, 그리고 여러 메타정보를 가지고 있는 csv file이 존재한다. 

csv file의 각 column은 다음과 같다.
> * Focus - Pet stands out against uncluttered background, not too close / far.
> * Eyes - Both eyes are facing front or near-front, with at least 1 eye / pupil decently clear.
> * Face - Decently clear face, facing front or near-front.
> * Near - Single pet taking up significant portion of photo (roughly over 50% of photo width or height).
> * Action - Pet in the middle of an action (e.g., jumping).
> * Accessory - Accompanying physical or digital accessory / prop (i.e. toy, digital sticker), excluding collar and leash.
> * Group - More than 1 pet in the photo.
> * Collage - Digitally-retouched photo (i.e. with digital photo frame, combination of multiple photos).
> * Human - Human in the photo.
> * Occlusion - Specific undesirable objects blocking part of the pet (i.e. human, cage or fence). Note that not all blocking objects are considered occlusion.
> * Info - Custom-added text or labels (i.e. pet name, description).
> * Blur - Noticeably out of focus or noisy, especially for the pet’s eyes and face. For Blur entries, “Eyes” column is always set to 0.

### 2) Evaluation
![image](https://github.com/hyunyongPark/Kaggle_petfinder/blob/main/imgs/evaluation.PNG)

본 대회에서는 RMSE 산식을 이용하여 리더보드 평가를 진행한다. 

<br/><br/><br/>
# Solution
### 1) modeling

### 2) Ensemble



<br/><br/><br/>
# Conclusion
원래 public 리더보드는 80등 은메달권에 정착하고 있었으나, 마지막 private 리더보드에서 530등(Top 15%) 획득하였다. public의 경우 테스트데이터의 25%, private는 75%로 평가를 하는데, 이렇게 25% 데이터에 대해 오버피팅이 심하게 발생할지는 예상하지 못했다. noise가 심한것일까.. 대회자체가 많은 의문이 드는 대회였던것 같다..

**public**
![image](https://github.com/hyunyongPark/Kaggle_petfinder/blob/main/imgs/leaderboard_private.PNG)

**private**
![image](https://github.com/hyunyongPark/Kaggle_petfinder/blob/main/imgs/leaderboard_public.PNG)
