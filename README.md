# S3CavVineyardDataset
Labeled images from vineyards in Switzerland

## Dataset description
This dataset is made of natural images acquired in-field by the Intel RealSense R200 (Santa Clara, CA, USA) RGB-D camera. The resolution of the color images has been set to 640×480 pixels as the maximum achievable resolution of the depth maps (not included in this dataset).

The Intel RealSense R200 is on a mobile platform (Niko caterpillar, Bühl/Baden, Germany), guided in a commercial vineyard of a white variety of wine grape (Räuschling) in Switzerland (N47°14’27.6”, E8°48’25.2”). Datasets were completed in two days of acquisitions, during which the vehicle followed specific paths within the parallel rows of grapes (row spacing between 1.5 and 2 m) at an average speed of 1.5 m/s. The camera pointed laterally at the rows of grapevines at a distance in the range between 0.75 and 1 m, producing video streams at a framerate of 5 fps. 

Among the whole set of images, 85 were manually annotated for semantic segmentation. Corresponding ground truth maps are in false colors, referring to five classes of interest:
-	Bunch class (white segments): grapevine bunches;
-	Pole class (red segments): vineyard poles;
-	Wood class (blue segments): wooden parts of the grapevines, such as trunks and cordons;
-	Leaves class (green segments): leaves;
-	Background class (black segments): pixels not belonging to none of the previous classes.

Labeled images are already divided into training and test sets to produce results comparable with the refencences [1], [2], and [3]. 
Two annotation strategies have been followed to produce two sets of labels:
-	Bunch/leaves-detection-oriented (BLDO): all pixels belonging to the grapevine bunches and leaves are labeled with the highest priority vs. the other classes. This dataset is used in [1], [2], and [3] and well-applies for targets of yield estimation and/or biomass monitoring;lines);
-	Object-segmentation-oriented (OSO): images are labeled assuming that all classes have the same relevance.Labeling is performed to segment what eyes can see. This dataset is used in [3].

## Acknowledgments
This work is funded by the project S3-CAV "Simultaneous Safety and Surveying for Collaborative Agricultural Vehicles", ERA-NET ICT-AGRI2 (Grant No. 29839).

## Credits
Experiments were conceived and performed by Annalisa Milella (CNR-STIIMA) and Giulio Reina (Politecnico of Bari). Roberto Marani (CNR-STIIMA) and Antonio Petitti (CNR-STIIMA) contributed to dataset generation and maintenance by software development and data processing. The valuable support of Stefan Rilling (Fraunhofer-IAIS), Michael Nielsen (Danish Technological Institute) and Peter Frölich (AgriCircle) in performing the experiments and gathering the sensory data is also gratefully acknowledged.

Contact person: Annalisa Milella - annalisa.milella@stiima.cnr.it

National Research Council of Italy (CNR), Institute of Intelligent Systems and Technologies for Advanced Manufacturing (STIIMA), via Amendola 122 D/O, 70126, Bari, Italy

## Cite this dataset
-	Milella, A., Marani, R., Petitti, A., Reina, G. (2019) In-field high throughput grapevine phenotyping with a consumer-grade depth camera. Computers and Electronics in Agriculture, 156, 293-306.

## References
1. Marani, R., Milella, A., Petitti, A., & Reina, G. (2021). Deep neural networks for grape bunch segmentation in natural images from a consumer-grade camera. Precision Agriculture, 22(2), 387-413.
2. Heras, J., Marani, R., & Milella, A. (2021). Semi-supervised semantic segmentation for grape bunch identification in natural images. In Precision agriculture’21 (pp. 65-84). Wageningen Academic Publishers.
3. Casado-García, A., Heras, J., Milella, A., & Marani, R. (2022). Semi-Supervised Deep Learning and Low-Cost Cameras for the Semantic Segmentation of Natural Images in Viticulture. Precision Agriculture 23, 2001–2026 https://doi.org/10.1007/s11119-022-09929-9
