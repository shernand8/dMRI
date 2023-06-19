# Neonatal Brain White Matter Development Evaluation using dMR

## Summary


## Background


## Method

### Data 

For this experiment, data was obtained from 489 babies some of which were born prematurely. The data used includes the following: 

* dMRI scans 
* Gestational ages 
* Age at which babies were scanned
* Head circumference when scanned
* Weight at birth

The gestational ages of babies scanned between 40 and 41 weeks are shown in the following distribution. 

![Gestational Age Distribution](https://drive.google.com/uc?id=1LCd1YB8YDyCEmqMZCM0EvNPkMUssbpJb) 

The birth weights of babies scanned between 40 and 41 weeks are shown in the following distribution. 

![Birth Age Distribution](https://drive.google.com/uc?id=1-BBC-bT_xpat5GRlipMJzbpPlEcna2aN)

### Experiment 1: use k-means to classify the data 

In this experiment, a scatter plot of head circumference when scanned and age when scanned was graphed. 

![Single Color Scatter](https://drive.google.com/uc?id=1cIFhH1HASVNz49xkZYz9YDaMRgJ4k18f)

This plot includes the data from 487 babies, excluding the data of babies whose head circumferences were not provided. 

To classify the data using k-means, the KMeans library was imported. To use this code, an array of every data entry must be defined. After this has been done, the KMeans function was used to set the number of clusters to three. Then the labels for each data entry were printed. 

### Results 

The classification result for the entire dataset is shown in the following figure. 

![First Classification Result](https://drive.google.com/uc?id=1efW8intCY-An-45jMErLoqx51xpKzIhu) 

These results are not what we expected. When we selected clusters according to birth age ranges, we obtained the following clusters. 

![Expected Classification Result](https://drive.google.com/uc?id=1-TZJxv_yPWlQjqlcKh-3MrE7LTEb5pqF) 

The expected clusters are very different from the clusters obtained using k-means. This means that the data entries were more closely related by a factor that was not our choses birth age ranges. We may have obtained these results because birth age range cannot be predicted easily from scan head circumference and from birth weight, especially considering that the babies were scanned at varying times following their births. It is also possible that the age ranges we used affected our results since we grouped moderate and late preterms together as well as extreme and very preterms together. 

## Reproducibility
### Dependencies

* numpy
* sklearn.cluster
* pandas
* matplotlib
* Overleaf
* Markdown
* Github
* Google colab
