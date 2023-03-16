## Tracking Early Mammalian Organogenesis – Prediction and Validation of Differentiation Trajectories at Whole Organism Scale


**Ivan Imaz-Rosshandler<sup>1,2,3,\*</sup>, Christina Rode<sup>4,\*</sup>, Carolina Guibentif<sup>5,\*</sup>, Mai-Linh Ton<sup>1,2</sup>, Parashar Dhapola<sup>10</sup>, Daniel Keitley<sup>6</sup>, Ricard Argelaguet<sup>11,12</sup>, Fernando J. Calero-Nieto<sup>2</sup>, Jennifer Nichols<sup>2</sup>, John C. Marioni<sup>7,8,9,\*\*</sup>, Marella de Bruijn<sup>4,\*\*</sup>, Berthold Göttgens<sup>1,2,\*\*</sup>**

### Table of Contents

1. [Paper abstract](#Abstract)
2. [Data availability](#data)
3. [Explore the data](#explore)
4. [Code availability](#code)
5. [Contact](#contact)
6. [Other links](#links)

   

### Abstract

Early organogenesis represents a key step in animal development, where pluripotent cells divide and diversify to initiate formation of all major organs. Here, we used scRNA-Seq to profile over 300,000 single cell transcriptomes sampled in 6 hour intervals from mouse embryos between E8.5 and E9.5. Combining this dataset with our previous E6.5 to E8.5 atlas resulted in a densely-sampled time course of over 400,000 cells from early gastrulation to organogenesis. Computational lineage reconstruction at full organismal scale identified complex waves of blood and endothelial development, including a new molecular programme for somite-derived endothelium. To assess developmental fates across the primitive streak, we dissected the E7.5 primitive streak into four adjacent regions, performed scRNA-Seq and predicted cell fates computationally. We next defined early developmental state/fate relationships experimentally by a combination of orthotopic grafting, microscopic analysis of graft contribution as well as scRNA-Seq to transcriptionally determine cell fates of the grafted primitive streak regions after 24h of in vitro embryo culture. Experimentally determined fate outcomes were in good agreement with the fates predicted computationally, thus demonstrating how classical grafting experiments can be revisited to establish high-resolution cell state/fate relationships. Such interdisciplinary approaches will benefit future studies in both developmental biology as well as guide the in vitro  production of cells for organ regeneration and repair.

### Data availability<a name="data" />

This data is an extension of a previously reported scRNA-Seq atlas covering mouse gastrulation and the early initiation of organogenesis through a densely sampled time-course of 6h sampling intervals from E6.5 to E8.5 (Pijuan-Sala B., Griffiths J. A., Guibentif C. et al., 2019) with newly sampled time points (E8.75-E9.5) as well as one overlapping time point (E8.5) to facilitate data integration. Combined, the new ‘extended’ atlas, ranging from E6.5 to E9.5 contains 430,339 cells across 13 time points spanning 3 days of mouse development 

Various forms of the transcriptomics data such as raw counts, normalised counts, dimensionality reductions and metadata are available [here](https://cloud.mrc-lmb.cam.ac.uk/s/yxq7FRtYsLyF3jQ) for loading into R and python. 


| File name                                                    | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| `embryo_counts.h5ad`                                                | AnnData object with UMI counts and metadata for processing with [scanpy](https://scanpy.readthedocs.io/en/stable/index.html). Function read\_h5ad(filename, ...) is recommended. |
| `embryo_logcounts.h5ad`                                                  | AnnData object with log normalised UMI counts, metadata and batch corrected layouts. Function read\_h5ad(filename, ...) is recommended. |
| `embryo_sce.rds`                                                  | Contains a `SingleCellExperiment` object with counts, metadata and batch corrected layouts for processing in R. Pre-computed library size factors can be accessed to normalise the data. |
| `embryo_counts.tar.gz`                                               | Counts matrix in sparse format (`mtx`) with cell and gene metadata files. |
| `metadata_cells.csv`                                               | Cell metadata. |
| `metadata_genes.csv`                                               | Gene metadata, ensemble id and gene symbols. |
| `umap_layout.csv`                                               | UMAP layout. |
| `pca_batch_corrected.csv`                                               | Batch corrected PCA with MNN. |

Raw scRNA-seq files have been deposited in arrayexpress under the accession number E-MTAB-11763. For details of the other, externally generated datasets used in our analysis, see the methods section of the paper. 

Note: Smart-Seq2 data generated in this project will be soon made public.

### Explore the data<a name="explore" />

#### Shiny app 

The data can be explored after logging into [shiny app](http://extendedmouseatlas.com/).
 
IMPORTANT: This webpage is currently under development.

#### UCSC Cell browser

To be added soon. 

### Code availability<a name="code" />

To be added soon.


### Support or Contact<a name="contact" />

General queries can be directed to [Bertie Göttgens](mailto:bg200@cam.ac.uk) , [John Marioni](mailto:marioni@ebi.ac.uk). For issues relating to the data or code, you can email Ivan Imaz-Rosshandler at [ivanir@mrc-lmb.cam.ac.uk](mailto:ivanir@mrc-lmb.cam.ac.uk).


### Other links<a name="links" />

[Göttgens lab website](https://www.stemcells.cam.ac.uk/people/pi/gottgens)

[Marioni lab website](https://www.ebi.ac.uk/research-beta/marioni/)

[de Bruijn lab website](https://www.imm.ox.ac.uk/research/research-groups/de-bruijn-group-developmental-haematopoiesis)

[Shiny application of E6.5-E8.5 atlas of mouse gastrulation and early organogenesis](https://marionilab.cruk.cam.ac.uk/MouseGastrulation2018/)


###### Affiliations

1. *Department of Haematology, University of Cambridge, Cambridge CB2 0RE, UK*

2. *Wellcome-Medical Research Council Cambridge Stem Cell Institute, University of Cambridge, Cambridge CB2 0AW, UK*

3. *MRC Laboratory of Molecular Biology, Cambridge CB2 0QH, UK*

4. *MRC Molecular Haematology Unit, MRC Weatherall Institute of Molecular Medicine, Radcliffe Department of Medicine, University of Oxford, Oxford OX3 9DS, UK*

5. *Department of Microbiology and Immunology, University of Gothenburg, Gothenburg, Sweden*

6. *Department of Zoology, University of Cambridge, Cambridge CB2 3EJ, UK*

7. *Wellcome Sanger Institute, Wellcome Genome Campus, Saffron Walden CB10 1SA, UK*

8. *European Molecular Biology Laboratory, European Bioinformatics Institute, Saffron Walden CB10 1SA, UK*

9. *Cancer Research UK Cambridge Institute, University of Cambridge, Cambridge CB2 0RE, UK*

10. *Division of Molecular Hematology, Lund Stem Cell Center, Lund University, Sweden*

11. *Epigenetics Programme, Babraham Institute, Cambridge CB22 3AT, UK*

12. *Altos Labs Cambridge Institute, Granta Park, Cambridge, CB21 6GP, UK*


\* Authors contributed equally
\*\* Corresponding authors
   
