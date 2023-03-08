# Aidea-AOI
 CNN model for detecting defects on AOI images

此專案為藉由AOI影像訓練深度學習模型辨識產品表面瑕疵，使用框架為TensorFlow。結果顯示預訓練DenseNet模型的測試準確達到99.5%。

## 資料來源
AOI影像資料由工研院在Aidea釋出作為開放性議題，供參賽者建立瑕疵辨識模型。  
來源：https://aidea-web.tw/topic/a49e3f76-69c9-4a4a-bcfc-c882840b3f27

## 基本資訊
* 訓練資料：共2528張，並取其中20%作為驗證資料  
* 測試資料：共10142張  
* 影像類別：共6類(正常類別 + 5種瑕疵類別)  
* 影像尺寸：512x512  

## 資料前處理
* 影像水平、垂直平移0.05
* 影像隨機旋轉15度
* 影像大小縮為 224 x 224

## 使用模型
* InceptionResNet_v2
* Xception
* DenseNet169 

## 模型結果
![image](https://user-images.githubusercontent.com/102510341/223766452-53edbe46-d4ed-406d-ae44-8f298296f5d6.png)
![image](https://user-images.githubusercontent.com/102510341/223766432-65a48acd-f2cc-43c7-95af-be69e1e83738.png)


## 最終結果
將測試資料的預測結果上傳Aidea平台評分，10,142張測試資料的準確度達到99.5%，排名為15/494(Top2%)

![image](https://user-images.githubusercontent.com/102510341/223760567-e1913566-59b2-4cbd-a609-6904eb6257fa.png)
