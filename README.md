# Efficient-CovidNet : Covid-19 Detection from Chest X-Ray Images
### State of the art results for Covid-19 Detection from Chest X-Ray Images

The COVID-19 pandemic has wreaked havoc all over the world. The rising number of cases have overburdened healthcare systems even in the most developed countries. 
To ease the burden on healthcare systems we need a quick and efficient COVID-19 testing technique. Currently the RT-PCR ( Real-Time Reverse Transcription Polymerase Chain Reaction ) test 
is done to detect COVID-19 from respiratory samples (nasopharyngealor and pharyngeal swabs).  While the RT-PCR is the most accurate, it is a very time-consuming, laborious and complicated manual process. 
An alternative to this is coronavirus detection from Chest X-Ray images.  It has been discovered in studies that Chest X-Rays of COVID-19 patients have specific malformations that 
can be used to flag a positive corona case. Inspired by the work [COVID-Net](https://github.com/lindawangg/COVID-Net) by Linda Wang,  Zhong Qiu Lin and Alexander Wong, we use Deep Learning to detect 
coronavirus from Chest X-Ray images. To surpass previous results we use the EfficientNet-B1. Our model not only achieves +2\% accuracy, it also attains higher 
sensitivity and Positive Predictive Value than COVID-Net. The dataset we use is the open source COVIDx dataset.  It has approximately 14,000 X-Ray images. To the best of
our knowledge, this dataset contains the largest number of COVID-19 positive cases till date. Our goal is to push the Deep Learning community to create an efficient COVID-19 detector that can be used in the real world.

### Dataset 
We use the COVIDx Dataset. t is by far the most comprehensive and  largest  dataset  for  Chest  X-Ray  images.  It  contains a total of 13,975 Chest X-Ray Images 
across 13,870 patients. The dataset has 3 categories: normal, pneumonia (Non-COVID-19)  and COVID-19. The  dataset  is  completely  open  source. It can be created using code provided by authors of [COVID-Net](https://github.com/lindawangg/COVID-Net/blob/master/docs/COVIDx.md).
The version 3 of the dataset which we used can be downloaded from [here](https://www.kaggle.com/manan2m/covidx-v3).


