# Efficient-CovidNet : Covid-19 Detection from Chest X-Ray Images
### State of the art results for Covid-19 Detection from Chest X-Ray Images

The COVID-19 pandemic has wreaked havoc all over the world. The rising number of cases have overburdened healthcare systems even in the most developed countries. 
To ease the burden on healthcare systems we need a quick and efficient COVID-19 testing technique. Currently the RT-PCR ( Real-Time Reverse Transcription Polymerase Chain Reaction ) test is done to detect COVID-19 from respiratory samples (nasopharyngealor and pharyngeal swabs).  While the RT-PCR is the most accurate, it is a very time-consuming, laborious and complicated manual process. 
An alternative to this is coronavirus detection from Chest X-Ray images.  It has been discovered in studies that Chest X-Rays of COVID-19 patients have specific malformations that 
can be used to flag a positive corona case. Inspired by the work [COVID-Net](https://github.com/lindawangg/COVID-Net) by Linda Wang,  Zhong Qiu Lin and Alexander Wong, we use Deep Learning to detect 
coronavirus from Chest X-Ray images. To surpass previous results we use the EfficientNet-B1. Our model not only achieves +2\% accuracy, it also attains higher 
sensitivity and Positive Predictive Value than COVID-Net. The dataset we use is the open source COVIDx dataset.  It has approximately 14,000 X-Ray images. To the best of
our knowledge, this dataset contains the largest number of COVID-19 positive cases till date. Our goal is to push the Deep Learning community to create an efficient COVID-19 detector that can be used in the real world.

## Dataset 
We use the COVIDx Dataset. t is by far the most comprehensive and  largest  dataset  for  Chest  X-Ray  images.  It  contains a total of 13,975 Chest X-Ray Images 
across 13,870 patients. The dataset has 3 categories: normal, pneumonia (Non-COVID-19)  and COVID-19. The  dataset  is  completely  open  source. It can be created using code provided by authors of [COVID-Net](https://github.com/lindawangg/COVID-Net/blob/master/docs/COVIDx.md).
The version 3 of the dataset which we used can be downloaded from [here](https://www.kaggle.com/manan2m/covidx-v3).


<p align="center">
  <img src="https://github.com/mananm98/Efficient-CovidNet/blob/master/images/Screen%20Shot%202020-08-21%20at%2020.12.04.png" />
</p>

<p align="center"> Example of COVIDx Dataset  </p>

## Results

### Test Accuracy (%)
|   **Architecture**  | **Test Accuracy** |
|:---------------:|---------------|
| EfficientNet-B1 |       **95**      |
|      VGG-19     |      83.0     |
|    Resnet-50    |      90.6     |
|     COVIDNet    |      93.3     |


### Sensitivity (%)
| **Architecture** | **Normal** | **Non-COVID-19** | **COVID-19** |
|:----------------:|:----------:|:----------------:|:------------:|
|  EfficientNet-B1 |    95.5    |     **94.6**     |    **100**   |
|      VGG-19      |  **98.0**  |       90.0       |     58.7     |
|     Resnet-50    |    97.0    |       92.0       |     83.0     |
|  COVIDNet-CXR4-A |    94.0    |       94.0       |     95.0     |
|  COVIDNet-CXR4-B |    96.0    |       92.0       |     93.0     |
|  COVIDNet-CXR4-C |    95.0    |       89.0       |     96.0     |


### Positive Predictive Value (%)
| **Architecture** | **Normal** | **Non-COVID-19** | **COVID-19** |
|:----------------:|:----------:|:----------------:|:------------:|
|  EfficientNet-B1 |  **93.5**  |     **96.9**     |     94.3     |
|      VGG-19      |    83.1    |       75.0       |     98.4     |
|     Resnet-50    |    88.2    |       86.8       |     98.8     |
|  COVIDNet-CXR4-A |    91.3    |       93.1       |   **99.0**   |
|  COVIDNet-CXR4-B |    88.9    |       93.9       |     98.9     |
|  COVIDNet-CXR4-C |    90.5    |       93.7       |     96.0     |
