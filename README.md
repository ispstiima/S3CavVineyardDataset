# S3CavVineyardDataset
Labeled images from vineyards in Switzerland

## Dataset description
This dataset is made of natural images acquired in-field by the Intel RealSense R200 (Santa Clara, CA, USA) RGB-D camera. The resolution of the color images has been set to 640×480 pixels as the maximum achievable resolution of the depth maps (not included in this dataset).

The Intel RealSense R200 is on a mobile platform (Niko caterpillar, Bühl/Baden, Germany), guided in a commercial vineyard of a white variety of wine grape (Räuschling) in Switzerland (N47°14’27.6”, E8°48’25.2”). Datasets were completed in two days of acquisitions, during which the vehicle followed specific paths within the parallel rows of grapes (row spacing between 1.5 and 2 m) at an average speed of 1.5 m/s. The camera pointed laterally at the rows of grapevines at a distance in the range between 0.75 and 1 m, producing video streams at a framerate of 5 fps. 

Among the whole set of images, 84 were manually annotated for semantic segmentation. Corrsponding ground truth maps are in false colors, referring to five classes of interest:
-	Bunch class (white segments): all pixels belonging to the grapevine bunches (of main interest along these lines);
-	Pole class (red segments): all pixels belonging to the vineyard poles;
-	Wood class (blue segments): all pixels belonging to wooden parts of the grapevines, such as trunks and cordons;
-	Leaves class (green segments): all pixels whose appearance can be referred to leaves;
-	Background class (black segments): all pixels not belonging to none of the previous classes.

Labeled images are already divided into training and test sets to produce results comparable with the refencences [1], [2], and [3].

## Acknowledgments
This work is funded by the project S3-CAV "Simultaneous Safety and Surveying for Collaborative Agricultural Vehicles", ERA-NET ICT-AGRI2 (Grant No. 29839). The authors are also grateful to Stefan Rilling, Peter Frölich and Michael Nielsen for the valuable support in performing the experiments and gathering the sensory data.

## Credits


## Cite this dataset
Milella, A., Marani, R., Petitti, A., Reina, G. (2019) In-field high throughput grapevine phenotyping with a consumer-grade depth camera. Computers and Electronics in Agriculture, 156, 293-306.

## References
1. Marani, R., Milella, A., Petitti, A., & Reina, G. (2021). Deep neural networks for grape bunch segmentation in natural images from a consumer-grade camera. Precision Agriculture, 22(2), 387-413.
2. Heras, J., Marani, R., & Milella, A. (2021). Semi-supervised semantic segmentation for grape bunch identification in natural images. In Precision agriculture’21 (pp. 65-84). Wageningen Academic Publishers.
3. To be completed
