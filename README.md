# covid_ml
CovidML model
Made an ML model to predict 3 classes

- Covid
- pneumonia
- normal

Used the [`COVID19_Pneumonia_Normal_Chest_Xray_PA_Dataset`](https://www.kaggle.com/datasets/amanullahasraf/covid19-pneumonia-normal-chest-xray-pa-dataset) from [Kaggle](https://www.kaggle.com)

This dataset is quite popular. It has also been employed in [this paper](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0265949) published in [PLoS One.](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8982897/#) 2022

<aside>
🔢 Applied `Transfer Learning`
</aside>

Used the pre-trained weights of the VGG19. Added a few layers on top of that.

Performed the ML workflow. 

1. pre-processing
2. normalising
3. creating the architecture
4. training
5. evaluating

|FIELD1|Class Name|precision|recall|f1-score|support|
|------|----------|---------|------|--------|-------|
|0     |covid     |0.9930   |0.9661|0.9794  |295    |
|1     |normal    |0.9099   |0.9734|0.9406  |301    |
|2     |pneumonia |0.9757   |0.9336|0.9542  |301    |



### Train Accuracy
![image](https://user-images.githubusercontent.com/85307430/235783583-8739b84d-0a43-4012-ba1d-f43e9a580c44.png)


### Loss
![loss](https://user-images.githubusercontent.com/85307430/235784242-f6cf5e37-f664-461f-89d3-8abcb932c7b2.jpeg)


## Confusion Matrix

### not normalised
![cf](https://user-images.githubusercontent.com/85307430/235784314-cb53f84b-f6a9-4879-8f25-e76e93934e73.jpeg)

### normalised
![normal](https://user-images.githubusercontent.com/85307430/235784345-acb8c952-6a78-4285-85c7-e5b2eae22884.jpeg)
