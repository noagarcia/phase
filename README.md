## PHASE: Demographic Annotations on the GCC Dataset

This is a repository for PHASE,  a set of annotations to study demographic bias on uncurated text-image datasets. PHASE (Perceived Human Annotations for Social Evaluation) have been annotated with demographic and contextual attributes on images from the [Google Conceptual Captions](https://ai.google.com/research/ConceptualCaptions/) dataset. 

PHASE is described in the paper "Uncurated Image-Text Datasets: Shedding Light on Demographic Bias" by *Noa Garcia, Yusuke Hirota, Yankun Wu,* and *Yuta Nakashima*. To appear soon.

### News

- **Mar. 2023**: PHASE has been selected as a highlight paper at CVPR 2023.
- **Feb. 2023**: PHASE has been accepted at CVPR 2023.


## Collection process
For a subset of the GCC images:
1. We detect regions with people with YOLOv5.
2. We filter the regions to discard missdections.
3. Annotators annotate 4 demographic and 2 contextual attibutes per region.
4. Each attribute is annotated by 3 different annotators.

<p align="center">
  <img width="460" src="https://github.com/noagarcia/phase/blob/master/images/annotation_process.png.png">
</p>

## Download
Download images from [here](https://drive.google.com/file/d/1-GGvJjkIrDjQlSnoPmOKY3KqCeeGyDGT/view?usp=share_link).
Download annotations from [here](https://drive.google.com/file/d/1COJCqMj4Jdj7Vu_87uJ4tKaQZyGISMTm/view?usp=share_link). The zip file contains the following files:

- All the annotations (3 annotations per region-attribute):
  - `phase_gcc_val_all_20221101.json`
  - `phase_gcc_train_all_20221101.json`

- Region-level annotations (1 annotation per region-attribute after majority voting):
  - `phase_gcc_val_regions_20221101.json`
  - `phase_gcc_train_regions_20221101.json`

- Annotators information:
  - `annotators.csv`

## Important information

### Intended uses

The dataset can only be used for research purpose. No commercial applications are allowed.
Annotators can revoke their consent to share their data at any point by contacting us. 

### Reference
 
If you find PHASE useful, please cite our research paper:

````
@InProceedings{garcia2023uncurated,
   author    = {Noa Garcia and Yusuke Hirota and Yankun Wu and Yuta Nakashima},
   title     = {Uncurated Image-Text Datasets: Shedding Light on Demographic Bias},
   booktitle = {CVPR},
   year      = {2023},
}
````

