## Tracking Early Mammalian Organogenesis – Prediction and Validation of Differentiation Trajectories at Whole Organism Scale

**List of authors to be added** 


### Table of Contents

1. [Paper abstract](#Abstract)
2. [Data availability](#Data-availability)
3. [Explore the data](#Explore-the-data)
4. [Code availability](#Code-availability)
5. [Contact](#Support-or-Contact)
6. [Other links](#Other-links)

   

### Abstract

Early organogenesis represents a key step in animal development, whereby pluripotent cells divide and diversify to initiate formation of all major organs. Tracking the underlying processes represents a fundamental question in developmental biology, with implications for producing authentic cell types in vitro and in vivo organ regeneration and repair. Here, we report over 300,000 new single cell RNA-Seq (scRNA-Seq) transcriptomes sampled in 6 hour intervals from mouse embryos between E8.5 and E9.5 days of development. Combining this dataset with our previous E6.5 to E8.5 atlas resulted in a densely-sampled time course of over 400,000 cells from early gastrulation to organogenesis. We performed computational lineage reconstruction at full organismal scale, which identified complex waves of blood and endothelial development revealing their distinct molecular programmes. To anchor computational cell fate predictions in experimentation, we dissected the E7.5 primitive streak into four sequential segments, and showed fates predicted from scRNA-Seq were in good agreement with the known fate outcomes of different primitive streak portions. To further define early developmental state / fate relationships, we performed orthotopic transplantation of primitive streak segments followed by 24h static in vitro embryo culture and assessed grafted cells based on morphological observation of cell type contribution and scRNA-Seq. Taking advantage of both ubiquitous and lineage-specific reporter genes, we show how a comprehensive single cell atlas provides a powerful resource to revisit classical grafting experiments to establish high-resolution cell state / fate relationships. Our study thus reports a resource coupled with an interdisciplinary approach to advance both conventional developmental biology as well as regenerative medicine.

### Data availability

This data is an extension of a previously reported scRNA-Seq atlas covering mouse gastrulation and the early initiation of organogenesis through a densely sampled time-course of 6h sampling intervals from E6.5 to E8.5 (Pijuan-Sala B., Griffiths J. A., Guibentif C. et al., 2019) with newly sampled time points (E8.75-E9.5) as well as one overlapping time point (E8.5) to facilitate data integration. Combined, the new ‘extended’ atlas, ranging from E6.5 to E9.5 contains 430,339 cells across 13 time points spanning 3 days of mouse development 

Various forms of the transcriptomics data are available [here](to be located at JCBC or UCSC server) for loading into R and python. 
| File name                                                    | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| `data.h5ad`                                                | AnnData object with raw counts for processing with [scanpy](https://scanpy.readthedocs.io/en/stable/index.html). |
| `data_processed.h5ad`                                                  | AnnData object with log normalised counts, metadata and main batch corrected layouts. |
| `sce.rds`                                                  | Contains a `SingleCellExperiment` object for processing in R. |
| `counts.mtx`                                               | Counts matrix in MatrixMarket format                         |
| `logcounts.mtx`                                            | Normalised logcounts in MatrixMarket format                  |
| `meta.tsv`                                                 | Per-cell observations (e.g. sample, cell type annotation, stage) |
| `genes.tsv`                                                | Ensembl codes and gene names for the scRNA-seq features.     |
| `sizefactors.tsv`                                          | Normalisation size factors computed for each cell using scran. |
| `corrected_pcs.tsv`                                        | The top 50 principal components resulting from fastMNN batch correction. |
| `r_umap.tsv` `r_tsne.tsv` `r_fa.tsv` `r_umap3d.tsv` | List of DataFrames containing coordinates for reduced dimensionality representations (e.g. UMAP, TSNE, PCA). |

Raw scRNA-seq files have been deposited in arrayexpress under the accession number E-MTAB-11763 (This project is under curation and will remain temporarly private). For details of the other, externally generated datasets used in our analysis, see the methods section of the paper. 

### Explore the data

#### Scarf web

The data can be explored after logging into [scarfweb](https://scarfweb.app/) using the following credentials (this is a temporary requirement):

User: mouseatlas \\
Password: Mouseatlas123

Once logged into scarfweb, the Mouse Extended Atlas can be explored using the following link
 [MouseEmbryoScarf](https://scarfweb.app/#/explorer/65fce9c2-2cc0-48b2-9376-7cbd9115f1a5).
 
IMPORTANT: This is a Beta version of Scarf Web and does not represent final quality. The upcoming release will include several new fatures.

#### Shiny app 

To be added. 

### Code availability

To be added.

### Support or Contact

General queries can be directed to [Bertie Göttgens](bg200@cam.ac.uk) , [John Marioni](mailto:marioni@ebi.ac.uk). For issues relating to the data, code or scarfweb app, you can email Ivan Imaz-Rosshandler at [ivanir@mrc-lmb.cam.ac.uk](mailto:ivanir@mrc-lmb.cam.ac.uk). 

### Other links

[Göttgens lab website](https://www.stemcells.cam.ac.uk/people/pi/gottgens)

[Marioni lab website](https://www.ebi.ac.uk/research-beta/marioni/)

[de Bruijn lab website](https://www.imm.ox.ac.uk/research/research-groups/de-bruijn-group-developmental-haematopoiesis)

###### Affiliations

1. *Department of Haematology, University of Cambridge, Cambridge, UK*

2. *Wellcome-Medical Research Council Cambridge Stem Cell Institute, University of Cambridge, Cambridge, UK*

3. *Department of Zoology, University of Cambridge, Cambridge, UK*

4. *Department of Microbiology and Immunology, University of Gothenburg, Gothenburg, Sweden*

5. *Department of Pathology & Imaging, Novo Nordisk, Måløv, Denmark*

6. *Medical Research Council Laboratory of Molecular Biology, Cambridge, UK*

7. *Wellcome Sanger Institute, Wellcome Genome Campus, Cambridge, UK*

8. *European Molecular Biology Laboratory European Bioinformatics Institute, Cambridge, UK*

9. Cancer Research UK Cambridge Institute, University of Cambridge Cambridge, UK

   \* Authors contributed equally

   
