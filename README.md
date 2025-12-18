# Description
This repo contains code used to analyse single-cell RNA-seq datasets of IkBa KO and wt mice (colon and spleen) to uncover properties of immune cells in these conditions. Data was obtained in collaboration with Luisa Barleben (Marina Kolesnichenko's Lab).

Short summary of the manuscript: "Epithelial NF-κB signaling plays a paradoxically protective role in colitis. Using ulcerative colitis (UC) patient biopsies and mouse models, we show that NF-κB-driven pro-inflammatory signals from intestinal epithelial cells recruit regulatory T cells and aid recovery. In UC, NF-κB selectively activates genes that shape immune responses. These findings uncover a key epithelial mechanism essential for resolving inflammation."

# Dependencies 
If you're working in R the following packages are required. You can install them using the command below:
```
install.packages(c("data.table", "ggplot2", "ggpubr", "pbapply", "ggrepel", "pheatmap", "openxlsx", "effectsize", "BiocManager", "devtools", "Seurat", "gprofiler2", "stringr", "pheatmap", "ggrepel", "ggridges"))
BiocManager::install(c("RUVSeq", "EDASeq", "DESeq2", "progeny", "singscore", 'celldex', 'SingleR', 'AUCell', 'BiocParallel', 'ComplexHeatmap'))
devtools::install_github('immunogenomics/presto') #optional, makes marker finding in Seurat extra fast 
devtools::install_github("jinworks/CellChat") 
```

If you're working in Python:
```
# Install libraries

!pip install scanpy
!pip install harmonypy
!pip install leidenalg
!pip install h5py
!pip install gseapy
!pip install crc32c

# Import packages

import os
import scanpy as sc
import scanpy.external as sce
import harmonypy as hm
from itertools import combinations
import pandas as pd
import gseapy as gp
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from scipy.stats import kruskal
```
