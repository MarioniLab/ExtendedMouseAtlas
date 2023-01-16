## Tracking Early Mammalian Organogenesis – Prediction and Validation of Differentiation Trajectories at Whole Organism Scale


**Ivan Imaz-Rosshandler<sup>1,2,3,\*</sup>,Christina Rode<sup>4,\*</sup>,Carolina Guibentif<sup>5,\*</sup>,Mai-Linh Ton<sup>1,2</sup>,Parashar Dhapola<sup>10</sup>, Daniel Keitley<sup>6</sup>,Ricard Argelaguet<sup>11,12</sup>,Fernando J. Calero-Nieto<sup>2</sup>,Göran Karlsson<sup>10</sup>, Marella de Brujin<sup>4</sup>, John Marioni<sup>7,8,9</sup>, Berthold Göttgens<sup>1,2</sup>**

### Table of Contents

1. [Paper abstract](#Abstract)
2. [Data availability](#data)
3. [Explore the data](#explore)
4. [Code availability](#code)
5. [Contact](#contact)
6. [Other links](#links)

   

### Abstract

Early organogenesis represents a key step in animal development, whereby pluripotent cells divide and diversify to initiate formation of all major organs. Tracking the underlying processes represents a fundamental question in developmental biology, with implications for producing authentic cell types in vitro and in vivo organ regeneration and repair. Here, we report over 300,000 new single cell RNA-Seq (scRNA-Seq) transcriptomes sampled in 6 hour intervals from mouse embryos between E8.5 and E9.5 days of development. Combining this dataset with our previous E6.5 to E8.5 atlas resulted in a densely-sampled time course of over 400,000 cells from early gastrulation to organogenesis. We performed computational lineage reconstruction at full organismal scale, which identified complex waves of blood and endothelial development revealing their distinct molecular programmes. To anchor computational cell fate predictions in experimentation, we dissected the E7.5 primitive streak into four sequential segments, and showed fates predicted from scRNA-Seq were in good agreement with the known fate outcomes of different primitive streak portions. To further define early developmental state / fate relationships, we performed orthotopic transplantation of primitive streak segments followed by 24h static in vitro embryo culture and assessed grafted cells based on morphological observation of cell type contribution and scRNA-Seq. Taking advantage of both ubiquitous and lineage-specific reporter genes, we show how a comprehensive single cell atlas provides a powerful resource to revisit classical grafting experiments to establish high-resolution cell state / fate relationships. Our study thus reports a resource coupled with an interdisciplinary approach to advance both conventional developmental biology as well as regenerative medicine.

### Data availability<a name="data" />

This data is an extension of a previously reported scRNA-Seq atlas covering mouse gastrulation and the early initiation of organogenesis through a densely sampled time-course of 6h sampling intervals from E6.5 to E8.5 (Pijuan-Sala B., Griffiths J. A., Guibentif C. et al., 2019) with newly sampled time points (E8.75-E9.5) as well as one overlapping time point (E8.5) to facilitate data integration. Combined, the new ‘extended’ atlas, ranging from E6.5 to E9.5 contains 430,339 cells across 13 time points spanning 3 days of mouse development 

Various forms of the transcriptomics data such as raw counts, normalised counts, dimensionality reductions and metadata are available [here](https://cloud.mrc-lmb.cam.ac.uk/s/yxq7FRtYsLyF3jQ) for loading into R and python. 
| File name                                                    | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| `embryo_scarfweb.h5ad`                                                | AnnData object with raw counts for processing with [scanpy](https://scanpy.readthedocs.io/en/stable/index.html). |
| `embryo_raw_counts.h5ad`                                                  | AnnData object with log normalised counts, metadata and main batch corrected layouts. |
| `embryo_sce.rds`                                                  | Contains a `SingleCellExperiment` object for processing in R. |
| `embryo_counts.rds`                                               | Counts matrix in sparse format for processing in R.                         |

Raw scRNA-seq files have been deposited in arrayexpress under the accession number E-MTAB-11763 (This project is under review and will remain temporarly private). For details of the other, externally generated datasets used in our analysis, see the methods section of the paper. 

### Explore the data<a name="explore" />

#### Scarf web

The data can be explored after logging into [scarfweb](https://scarfweb.app/) using the following credentials (this is a temporary requirement):

User: mouseatlas \\
Password: Mouseatlas123

Once logged into scarfweb, the Mouse Extended Atlas can be explored using the following link
 [MouseEmbryoScarf](https://scarfweb.app/#/explorer/65fce9c2-2cc0-48b2-9376-7cbd9115f1a5).
 
IMPORTANT: This is a Beta version of Scarf Web and does not represent final quality. The upcoming release will include several new fatures.

#### Shiny app 

To be added. 

### Code availability<a name="code" />

To be added.

### Support or Contact<a name="contact" />

General queries can be directed to [Bertie Göttgens](bg200@cam.ac.uk) , [John Marioni](mailto:marioni@ebi.ac.uk). For issues relating to the data, code or scarfweb app, you can email Ivan Imaz-Rosshandler at [ivanir@mrc-lmb.cam.ac.uk](mailto:ivanir@mrc-lmb.cam.ac.uk). 

### Other links<a name="links" />

[Göttgens lab website](https://www.stemcells.cam.ac.uk/people/pi/gottgens)

[Marioni lab website](https://www.ebi.ac.uk/research-beta/marioni/)

[de Bruijn lab website](https://www.imm.ox.ac.uk/research/research-groups/de-bruijn-group-developmental-haematopoiesis)

###### Affiliations

1. *Department of Haematology, University of Cambridge, Cambridge, UK*

2. *Wellcome-Medical Research Council Cambridge Stem Cell Institute, University of Cambridge, Cambridge, UK*

3. *MRC Laboratory of Molecular Biology, Cambridge, UK* 

4. *MRC Molecular Hematology Unit, MRC Weatherall Institute of Molecular Medicine, Raadcliffe Department of Medicine, University of Oxford, UK*

5. *Department of Microbiology and Immunology, University of Gothenburg, Gothenburg, Sweden*

6. *Department of Zoology, University of Cambridge, Cambridge, UK*

7. *Wellcome Sanger Institute, Wellcome Genome Campus, Cambridge, UK*

8. *European Molecular Biology Laboratory European Bioinformatics Institute, Cambridge, UK*

9. *Cancer Research UK Cambridge Institute, University of Cambridge Cambridge, UK*

10. *Division of Molecular Hematology, Lund Stem Cell Center, Lund University, Sweden*

11. *Epigenetics Programme, Babraham Institute, Cambridge CB22 3AT, UK*

12. *Altos Labs Cambridge Institute, Granta Park, Cambridge, CB21 6GP, UK*

\* Authors contributed equally

   
