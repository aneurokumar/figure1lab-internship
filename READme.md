# **Figure 1 Lab Internship Emulator**  
## **Introduction**
**Aims**  
The [Figure 1 Lab (F1L) Internship Emulator](https://github.com/deanslee/FigureOneLab/blob/main/README.md) is an self-paced, bioinformatics/computational biology internship emulated aimed at sealing the cracks in the Bioinfo/CompBio talent pipeline by working with real data in real papers, created by [Dean Lee](https://www.linkedin.com/in/deanslee/). The project aims to give students and professionals skills to work on bioinfo/compbio problems in the biotech landscape.  

**Key Scientific Question (KSQ)**  
<ins>The original KSQ is as follows:</ins>  
Using available scRNA-seq data from cancer cell lines, how would you explore the use of the following FDA-approved antibody therapies in additional cancers?  
- **Trastuzumab**: Targets HER2 and is used in the treatment of HER2-positive breast and gastric cancers.  
- **Bevacizumab**: Targets VEGF and is used for a variety of cancers, including colorectal, lung, glioblastoma, breast, liver, and kidney cancer.

<ins>Reformulated KSQ:</ins>  
Cancer cell lines have been used to develop antibody therapies against specific cancers thanks to scRNAseq data. How can we explore a cancer cell lines' scRNAseq data to reveal their underlying anomalies related to cell growth, maturation, proliferation, differentiation, and survival? Are the same proteins or protein-mediated pathways present in other cancers, where we can apply the same therapies developed for HER2 and VEGF?  

## **Mini-Literature Review**  

### <ins>**Definitions of main concepts**</ins>  

**Cancer and the use of cancer cell lines in research/therapies**  
At the cellular level, cancer is an anomoly of cell division, differentiation, and regulation. Cells have built in mechanisms to regulate their entire life cycle, and their failures result in seemingly endless proliferation, ignorance of surrounding cell signals, lack of self-induced death (apoptosis), and spreading to other healthy cells locally and throughout the body. [1] Cancer cells are often genetically heterogenous, rapid proliferation leading to mutations that lead to more rapid proliferation. A tumour can be composed of multiple cancerous cells with each cell having a different genetic makeup than its neighbors. Cancer drug treatments can be used to treat the abnormal mechanisms themselves. Kinker et al actually showed that several cancer cell lines share certain patterns in their transcriptomic profile, which suggests that we can draw similartities between seeingly "different diseases", and potentially use available medicines to    

**Single-cell RNA sequencing (scRNA-seq), and its potential and potential therapies**  
Traditional sequencing, or "bulk sequencing," gives us an average profile of cancer cells as a whole, but nuance is lost. Single-cell RNA sequencing data (scRNA-seq) provides the RNA sequencing inside individual cells, providing a live profile of the cells at the time of experiments. This data is particularly insightful for cancer cells, capable of showing a tumor's transciptomic profile of individual cells. This level of detail improves the research and creation of targeted therapies. 

### <ins>**HER2/VEGF, their mechanisms, and FDA-approved drug therpies**</ins>
**HER2 and Trastuzumab**  

- **HER2** transmembrane protein called human epidermal growth factor receptor 2, as well as an oncogene. HER2 is a member of a group of proteins called tyrosine kinase receptors, which have receptors on the cell surface and are important in cell signalling and cell regulation (division, movement, survival, etc.)[2]. HER2 overexpression is found in a subset of breast cancer, leading to hiigh proliferations and anti-cell death for diseased cells.  

- **Trastuzumab** is a recombinant humanized IgG1 monoclonal antibody that binds to HER2's extracellular receptor. Once bound, it blocks cleavage of HER2's extracellular domain, which triggers an inhibition of HER2-mediated signalling. Reduced HER2-mediated signalling leads to reduced cell growth and proliferation. It also attracts immune cells to tumor sites with overexpressed HER2 via antibody-dependent cell-mediated cytotoxicity. [6]  

**VEGF and Bevacizumab**  

- **VGEF** is a family of proteins called vascular endothelial growth factor, and is involved in regulating the formation of new blood vessels (angiogenesis). When overexpressed, VGEF can cause many abnormalities in the vascular/lymphatic system, which can directly affect not only cell regulation (as mentioned for HER2) but also the rate of metastasis - the spread and invasion of cancer cells to other parts of the body.[4] Abnormal angiogenesis is a tumor's wildest dream, because tumors need blood vessels for nutrients (including oxygen) to grow. Blood vessels formed from overexpressed VGEF are also "structurally and functionally abnormal," which can sometimes lead to a hypoxic state for tumors, causing a higher production of VGEF. [5]  

- **Bevacizumab** is a monoclonal Antibody (mAb) that binds to VGEF, leaving VGEF unable to interact with other receptors and therefore inhibiting its cell signalling capabilities. Reduced signalling means that its angiogenesis signalling is reduced, which prevents new bood vessels from forming and therefore reduces abnormal vasculor systems from forming around tumors.[7]  

## **Questions, ideas, and things to keep in mind**  
- **Cancer cell lines:** Cancer cell lines have a lot of experimental caveats to them - mutations introduced via high number of passaging, poor GLP practices, consistency of maintenance due to number of people performing it and their skill levels, etc. In vitro experiments aren't always going to be representative of in vivo experiments.
- **Data and what to look for:** Not having looked at the data or paper at this point, I don't know what format the data is in or what to look for in analysis. Dean mentioned resources [8] and [9] in the original LinkedIn post, so I'm keeping them in the resource list below and want to add a section in this memo about data analysis. These concepts came up while I was reading and might be worth looking into: c_opy number variation, epigenetic variation, extrachromosomal DNA distribution_
- **Different disease, same therapies:** In [7], the resource mentioned evidence of VEGF is also upregulated in COVID-19 patients, meaning that bevacizumab _could_ be used to treat a different disease. I'm tempted to look more closely at the mechanisms of VEGF and HER2, but worried I might get too lost in the weeds before starting the paper. I have those resources bookmarked and can always come back to them when needed to add more detail. 



 ## **Resources**  
1.  [Cooper GM. The Cell: A Molecular Approach. 2nd edition. Sunderland (MA): Sinauer Associates; 2000. The Development and Causes of Cancer.](https://www.ncbi.nlm.nih.gov/books/NBK9963/#:~:text=Cancer%20cells%20typically%20display%20abnormalities%20in%20the%20mechanisms,that%20regulate%20normal%20cell%20proliferation%2C%20differentiation%2C%20and%20survival.)  
2. [HER 2: Biology, Detection, and Clinical Implications - PMC (nih.gov)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3242418/#:~:text=The%20HER2%20pathway%20has%20been%20described%20in%20systems,that%20affect%20various%20cellular%20functions%20%288%29%20%28Fig.%201%29.)  
3. [Definition of receptor tyrosine kinase](https://www.cancer.gov/publications/dictionaries/cancer-terms/def/receptor-tyrosine-kinase#:~:text=reh%2DSEP%2Dter%20TY,movement%2C%20metabolism%2C%20and%20survival.)
4.  [Vascular Endothelial Growth Factor (VEGF) and Its Role in Non-Endothelial Cells: Autocrine Signalling by VEGF - Madame Curie Bioscience Database - NCBI Bookshelf](https://www.ncbi.nlm.nih.gov/books/NBK6482/#:~:text=Vascular%20endothelial%20growth%20factor%20(VEGF)%20is%20a%20potent%20angiogenic%20factor,tumor%20angiogenesis%20is%20well%20defined.)  
5. [VEGF as a Key Mediator of Angiogenesis in Cancer](https://karger.com/ocl/article-abstract/69/Suppl.%203/4/237877/VEGF-as-a-Key-Mediator-of-Angiogenesis-in-Cancer?redirectedFrom=fulltext)
6. [Trastuzumab mechanism of action for HER2](https://go.drugbank.com/drugs/DB00072)
7. [Bevacizumab mechanism of action for VEGF](https://go.drugbank.com/drugs/DB00112)





