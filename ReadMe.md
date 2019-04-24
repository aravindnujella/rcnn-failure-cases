# Curated List of Faster/MaskRCNN failure cases

Two main failure cases are 
1. Missing objects when the bounding boxes are similar

![](artefact1/resnet50_faster-rcnn_fpn/zebra1.png)
**Fig:** Missing Zebras with similar bounding boxes

![](artefact1/resnet50_faster-rcnn_fpn/000000537590.png)
**Fig:** Misslocalized airplanes


More Images of this type are in artefact1/. General feature of these artefacts is that there is either bad localization(i.e, bounding box predicted) or completely missed bounding boxes.

2. Lack of global context

![](artefact2/resneXt64_4d_mask-rcnn/000000150263.png)
**Fig:** laptop, chair predicted infront of train


More Images of this type are in artefact2/. These artefacts miss global context and misclassify some of the RoIs which a human wouldn't.

Examples from MSCOCO dataset for the similar artifacts are available at https://drive.google.com/open?id=1iPQNoTNqTuDhNECCX4j7aKkDZTPDTq3T