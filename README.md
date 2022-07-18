# GBDF: Gender Balanced DeepFake Dataset

<img src="images/maad_4_2.png" width="330" align="right" >

A publicly available gender-balanced and annotated deepfake dataset, GBDF, from FaceForensics++ (FF++), Celeb-DF, and Deeper Forensics-1.0 consisting of 10,000 live and fake videos generated using different identity and expression swapping deepfake generation techniques. The dataset consist of 10,000 videos with 5000 each for males and females with 1:4 real to fake ratio.
- [Research Paper]()
- [Download Data]()

Version 1.0 (07.17.2022)

## Table of Contents

- [Abstract](#abstract)
- [Database Properties](#database-properties)
- [Annotated Sample Images](#annotated-sample-images)
- [Download](#download)
- [Citing](#citing)
- [Acknowledgment](#acknowledgment)
- [License](#license)


## Abstract

Facial forgery by deepfakes has raised severe societal con-
cerns. Several solutions have been proposed by the vision community
to effectively combat the misinformation on the internet via automated
deepfake detection systems. Recent studies have demonstrated that fa-
cial analysis-based deep learning models can discriminate based on pro-
tected attributes such as gender and race. For the commercial adoption
and massive roll-out of the deepfake detection technology, it is vital to
evaluate and understand the fairness (the absence of any prejudice or fa-
voritism) of deepfake detectors across demographic variations (protected
attributes). As the performance differential of deepfake detectors between
demographic sub-groups would impact millions of people of the deprived
sub-group. This paper aims to evaluate the fairness of the deepfake de-
tectors across males and females. However, existing deepfake datasets are
not annotated with demographic labels to facilitate fairness analysis. To
this aim, we manually annotated existing popular deepfake datasets with
gender labels and evaluated the performance differential of current deep-
fake detectors across gender. Our analysis on the gender-labeled version
of the datasets suggests (a) current deepfake datasets have skewed dis-
tribution across gender, and (b) commonly adopted deepfake detectors
obtain unequal performance across gender with mostly males outper-
forming females. Finally, we contributed a gender-balanced and anno-
tated deepfake dataset, GBDF, to mitigate the performance differential
and to promote research and development towards fairness-aware deep
fake detectors
For more details, please take a look at the [Research Paper]().

## Database Properties

The GBDF dataset is created using FF++(c23 version), Celeb-DF, DeeperForensics-1.0 and consist of 10,000 videos with 5000 each for males and females.As none of these existing deepfake datasets contain demographic information, we manually annotated ground truth gender labels for these datasets. The gender annotated version of the live and deepfake videos from these deepfakes datasets are merged to create GBDF dataset.Deepfakes in the GBDF dataset are created using different Identity Swapping
(i.e., FaceSwap, FaceSwap-Kowalski, FaceShifter, Encoder-decoder style and End-
to-end Face Swapping techniques) and Expression swapping (i.e., Face2Face and
NeuralTextures) deepfake generation techniques. The majority of the videos in
GBDF are from Caucasians. The ratio of real to fake videos in the GBDF dataset
is 1 : 4. The GBDF is further divided into gender-balanced and subject inde-
pendent training and testing subsets in the ratio of 70 : 30.




## Download

[GBDF]() provides gender annotations for deepfakes of the [FaceForesincs++]() database,[Celeb-DF]() database,[Deeper Forensics-1.0]() database. 
- To get the **Deepfake dataset**, please visit the [VGGFace2 webside](http://www.robots.ox.ac.uk/~vgg/data/vgg_face2/data_infor.html) and download the images.
- The **Gender annotations** of GBDF dataset are stored under [releases](https://github.com/pterhoer/MAAD-Face/releases/tag/MAADFACE). 
The annotations can be downloaded either as csv or pickle file.
- The csv-file ("MAAD-Face.csv") provides the labels for a single image in each row. The first entry of the row specifies the filename of the face image, followed by an identity marker and the 47 attribute annotations. The first row provides information for the different column entries.
- The attribute files contain the gender annotations for the train of GBDF, in that order.





## Citing


If you use this work, please cite the following papers as well as the [VGGFace2](http://www.robots.ox.ac.uk/~vgg/data/vgg_face2) database.


```
@article{DBLP:journals/tifs/TerhorstFKDKK21,
  author    = {Philipp Terh{\"{o}}rst and
               Daniel F{\"{a}}hrmann and
               Jan Niklas Kolf and
               Naser Damer and
               Florian Kirchbuchner and
               Arjan Kuijper},
  title     = {MAAD-Face: {A} Massively Annotated Attribute Dataset for Face Images},
  journal   = {{IEEE} Trans. Inf. Forensics Secur.},
  volume    = {16},
  pages     = {3942--3957},
  year      = {2021},
  url       = {https://doi.org/10.1109/TIFS.2021.3096120},
  doi       = {10.1109/TIFS.2021.3096120},
  timestamp = {Thu, 16 Sep 2021 18:05:24 +0200},
  biburl    = {https://dblp.org/rec/journals/tifs/TerhorstFKDKK21.bib},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}

```

```
@inproceedings{DBLP:conf/btas/TerhorstHKZDKK19,
  author    = {Philipp Terh{\"{o}}rst and
               Marco Huber and
               Jan Niklas Kolf and
               Ines Zelch and
               Naser Damer and
               Florian Kirchbuchner and
               Arjan Kuijper},
  title     = {Reliable Age and Gender Estimation from Face Images: Stating the Confidence
               of Model Predictions},
  booktitle = {10th {IEEE} International Conference on Biometrics Theory, Applications
               and Systems, {BTAS} 2019, Tampa, FL, USA, September 23-26, 2019},
  pages     = {1--8},
  publisher = {{IEEE}},
  year      = {2019},
  url       = {https://doi.org/10.1109/BTAS46853.2019.9185975},
  doi       = {10.1109/BTAS46853.2019.9185975},
  timestamp = {Mon, 14 Sep 2020 18:11:03 +0200},
  biburl    = {https://dblp.org/rec/conf/btas/TerhorstHKZDKK19.bib},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```



## Acknowledgment

This work is supported in part from National Science Foundation (NSF) award
no. 2129173. The research infrastructure used in this study is supported in part
from a grant no. 13106715 from the Defense University Research Instrumentation
Program (DURIP) from Air Force Office of Scientific Research.


## License

This project is licensed under the terms of the Attribution-ShareAlike 4.0 International ([CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)) license.
All images used in this project belongs to the [VGGFace2](http://www.robots.ox.ac.uk/~vgg/data/vgg_face2). 
The copyright of the images remains with the original owners.
The copyright of the annotations remains with the Fraunhofer Institute for Computer Graphics Research IGD Darmstadt 2020.
