## Lung Nodule Texture and Malignancy Classification


Lung cancer classification in screening computed tomography (CT) scans is one of the most crucial tasks for early detection of this disease. Many lives can be saved if we are able to accurately classify malignant/cancerous lung nodules. Consequently, several deep learning based models have been proposed recently to classify lung nodules as malignant or benign. Nevertheless, the large variation in the size and heterogeneous appearance of the nodules makes this task an extremely challenging one.

## Dataset:

The Lung Image Database Consortium and Image Database Resource Initiative (LIDC-IDRI) database [7] is the largest publicly-available lung nodule dataset. It contains 1,018 computed tomography (CT) scans from 1,010 patients altogether collated from seven academic centers across the United States (US). The slice thicknesses of the CT scans range from 0.45 to 5.0 mm, as the scans were collated from different institutions and devices.

Each CT scan was annotated by four experienced thoracic radiologists altogether. We only used the nodules that were annotated by at least three out of four radiologists to ensure that the majority of radiologists agreed on the presence of a nodule. The four radiologists also rated each nodule on a scale of one to five, whereby one indicates that a nodule is clearly benign and five, clearly malignant. Therefore, to aggregate all of the malignancy ratings by all four radiologists, we took the median of the ratings of all four radiologists as the ground truth in our experiments. We excluded nodules with a median rating of 3 as we could not assign them to either benign or malignant groups. In this way, we obtained 848 nodules altogether, of which 442 were benign and 406 malignant

![Malignant and Benign Nodule in LIDC dataset](https://github.com/Azkarehman/Lung-Nodule-Classification/blob/main/fig/benign-malignant.png)

## Related Research

-   ProCAN: Progressive Growing Channel Attentive NonLocal Network for Lung Nodule Classification ([Link](https://arxiv.org/ftp/arxiv/papers/2010/2010.15417.pdf))
    
-   Automatic Categorization and Scoring of Solid, Part-Solid and Non-Solid Pulmonary Nodules in CT Images with Convolutional Neural Network([Link](https://www.nature.com/articles/s41598-017-08040-8.pdf))
 
- A Computer-Aided Pipeline for Automatic Lung Cancer Classification on Computed Tomography Scans ([Link](https://www.hindawi.com/journals/jhe/2018/9409267/))

## Results:

After multiple experimentation, we found the best suitable method for the problem. 
Cross fold validation was done and our results were reported to be 93.5%

