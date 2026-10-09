# UCSC Cell Browser Activity: From Genome to Cell

## 1. Assigned Gene and Disease
* **Student Name:** Gorgonio A. Aurea III
* **Student Number:** 202400706
* **Course:** Cell and Molecular Biology Laboratory
* **Assigned Gene Symbol:** ATP7A (ATPase Copper Transporting Alpha)
* **Associated Disease / Phenotype:** Menkes Disease
* **Reference Transcript:** NM_000052.7
* **Reference Protein:** NP_000043.4
* **Documented Variant:** c.2179G>A (p.Gly727Arg)
* **ClinVar Variation ID:** 210418

---

## 2. Organ/Tissue Choice and Dataset Information
* **Exact Dataset Name:** Adult Cortex Meta-Atlas
* **Organ/Tissue System:** Human Brain / Cerebral Cortex
* **Dataset URL:** https://cells.ucsc.edu/?ds=adult-cortex
* **Publication / Study Reference:** UCSC Cell Browser Collection (520,013 cells analyzed)
* **Rationale for Selection:** The cerebral cortex of the brain was chosen because Menkes disease is a severe X-linked recessive neurodegenerative disorder caused by loss-of-function mutations in the *ATP7A* gene. Impaired copper transport across the blood-brain barrier and within neural cells leads to severe developmental delay, seizures, cerebral atrophy, and early mortality.

<img width="720" height="1280" alt="01_dataset" src="https://github.com/user-attachments/assets/2a4eed75-c8cb-4d0b-99e0-dddcbb832db6" />


---

## 3. Understanding the Cell Map
* **Type of Visualization:** Dimensionality reduction scatter plot (UMAP/t-SNE layout).
* **What One Dot Represents:** One single measured cell (or nucleus) isolated from adult human cerebral cortex tissue.
* **What Clusters Represent:** Distinct cellular populations, cell lineages, or functional cell states that share similar overall transcriptomic (gene expression) profiles.
* **Visible Cell-Type/Cluster Labels:**
  1. **Glial & Vascular Cells:** Astrocyte, Oligodendrocyte, OPC (Oligodendrocyte Precursor Cells), Microglia, Endothelial, Pericyte, VLMC
  2. **Excitatory Neuronal Types:** IT (Intratelencephalic), L5 ET, L6 CT, L6b, L5/6 IT Car3
  3. **Inhibitory Neuronal Types:** SST, PVALB, VIP, LAMP5, PAX6

---

## 4. Assigned Gene Expression
* **Assigned Gene Symbol:** ATP7A
* **Dataset Used:** Adult Cortex Meta-Atlas (520,013 loaded cells)
* **Overall Expression Pattern:** Widespread but sparse across multiple cell clusters. Expression is detected at low-to-moderate levels in vascular and glial populations as well as select neuronal subtypes, with 97.9% of total cells displaying zero detected transcripts due to typical single-cell RNA-seq dropout and low baseline transcript abundance.
* **Clusters with Stronger Expression:** Endothelial, Pericyte, Astrocyte, and select Intratelencephalic (IT) cortical neurons (represented by dark purple/black dots in the 0.97 – 3.37 expression range).
* **Clusters with Little or No Detectable Expression:** Microglia and VLMC (showing predominantly baseline light blue/zero values).

<img width="720" height="1280" alt="02_gene_expression" src="https://github.com/user-attachments/assets/b5d5b98b-1719-4d74-84d3-af6ca625d359" />


---

## 5. Cell Types and Clusters
* **Cell type/cluster with strongest visible expression:** Endothelial and Pericyte cells (cerebral microvasculature).
* **Another cell type/cluster with detectable expression:** Astrocyte and IT (Intratelencephalic) neurons.
* **Cell type/cluster with relatively low or undetected expression:** Microglia.
* **Nature of Expression Pattern:** Broadly distributed across multiple cell lineages, though enriched in vascular/glial supporting cells and specific cortical neurons.
* **Biological Explanation:** ATP7A encodes a P-type ATPase copper transporter essential for cellular copper efflux and systemic copper homeostasis. In the central nervous system, ATP7A is heavily expressed in brain microvascular endothelial cells and astrocytes to transport copper across the blood-brain barrier into the brain parenchyma, as well as in neurons for cuproenzyme synthesis (e.g., cytochrome c oxidase and peptidylglycine alpha-amidating monooxygenase). In Menkes disease, loss of functional ATP7A impairs this transport at the blood-brain barrier and within neurons, resulting in severe local neurodegeneration.

<img width="720" height="1280" alt="03_cell_types" src="https://github.com/user-attachments/assets/ffc97c03-50ef-406b-aaaf-64a94481fbbf" />


---

## 6. Expression Plot
* **Selected Cells/Clusters Examined:** Cortical cell classes (IT, Astrocyte, Microglia, Endothelial, Pericyte, VLMC, etc.) across the Adult Cortex Meta-Atlas dataset.
* **Expression Comparison:** Vascular/supporting cells (Endothelial, Pericyte) and select neuronal lineages display higher average expression and higher proportions of non-zero expressing cells compared to background microglial and specific interneuron populations.
* **Value of the Expression Plot:** The dot plot quantifies both the relative average expression level (indicated by dot color intensity, range 0.01 – 0.03) and the percentage of cells within each cluster that actively express *ATP7A* (indicated by dot diameter). This resolves the expression frequency and baseline magnitude across cell classes far more clearly than visual density on the UMAP layout alone.

<img width="720" height="1280" alt="04_expression_plot" src="https://github.com/user-attachments/assets/8827f6c9-bd74-47df-86a6-1aa34ca8595e" />


---

## 7. Marker Genes
* **Cluster/Cell Type Examined:** Astrocyte
* **Marker Gene 1:** SLC1A3
* **Marker Gene 2:** AQP4
* **Marker Gene 3:** APOE
* **Behavior Comparison:** *ATP7A* does not behave as a cluster-specific marker gene in this dataset. While marker genes like *SLC1A3* or *AQP4* are highly specific to astrocytes (PCT1 > 0.78, high fold-change), *ATP7A* acts as a broad housekeeping/metabolic gene responsible for fundamental copper transport across multiple cell types rather than uniquely defining a single lineage.

<img width="720" height="1280" alt="05_marker_genes" src="https://github.com/user-attachments/assets/d2b92f07-8c09-488b-a717-152d73c3019d" />


---

## 8. Disease Gene vs. Marker Gene
* **Assigned Disease Gene:** ATP7A
* **Marker Gene:** AQP4 (Aquaporin 4)
* **More Cell-Type-Restricted Gene:** AQP4 (shows expression almost exclusively localized to astrocytes).
* **More Broadly Expressed Gene:** ATP7A (detectable across vascular, glial, and neuronal lineages).
* **Insight:** Disease-associated genes frequently encode essential metabolic, ion transport, or cellular maintenance proteins (such as copper ATPases) that are expressed broadly across multiple cell types, whereas cell-type marker genes encode highly specialized structural or lineage-specific functional proteins that uniquely define individual cell identities.

---

## 9. Connection to Genome Browser and ClinVar
1. **Chromosome Location:** Chromosome X (Xq21.1)
2. **Disease-Associated Variant Examined:** c.2179G>A (p.Gly727Arg), ClinVar ID: 210418
3. **Cell Types Expressing ATP7A:** Brain microvascular Endothelial cells, Pericytes, Astrocytes, and Intratelencephalic (IT) neurons.
4. **Biological Relevance:** Yes, this expression pattern aligns directly with Menkes disease pathology. ATP7A is critical in endothelial cells and astrocytes to transport copper across the blood-brain barrier into the brain parenchyma, and in neurons for vital cuproenzyme synthesis (such as cytochrome c oxidase). A loss-of-function mutation like p.Gly727Arg disrupts cellular copper transport, depriving neurons of essential copper and leading to severe progressive neurodegeneration.
5. **Single-Dataset Causality Proof:** No, a single Cell Browser dataset cannot prove causality. It only demonstrates observational transcript presence in specific cell populations; proving disease causality requires functional mutational assays, clinical genetic linkage, and biochemical validation of impaired copper transport mechanisms.

---

## 10. Reflection
1. **Genome Browser vs. Cell Browser:** The UCSC Genome Browser provided genomic coordinates, exon/intron gene structure, and specific DNA mutation (ClinVar) information. The UCSC Cell Browser built upon this by showing transcript distribution across distinct, functional single-cell populations in human tissue.
2. **Differential Expression Among Cell Types:** Different cell types express different gene regulatory networks and transcription factors based on their physiological function. Highly specialized cells upregulate specific metabolic pathways or structural proteins according to their role in tissue function.
3. **Caution with Zero/Low Expression:** Single-cell RNA-sequencing data suffers from high technical noise and dropout events, where lowly expressed transcripts are missed during sampling. A zero reading does not necessarily mean biological absence of mRNA or protein.
4. **Value of Multi-Omics Integration:** Combining genomic location, variant pathogenicity, and cell-type-specific expression provides a complete pathway view—from primary DNA mutation to cell lineage susceptibility and system-level phenotype.
5. **Most Interesting Observation:** Observing that *ATP7A* is strongly expressed in brain microvascular endothelial cells highlighted how Menkes disease neurodegeneration begins at the blood-brain barrier interface before affecting neural viability directly.

---

## 11. References and Links
* **UCSC Cell Browser:** https://cells.ucsc.edu/
* **Adult Cortex Meta-Atlas Dataset:** https://cells.ucsc.edu/?ds=adult-cortex
* **NCBI ClinVar (Variation ID 210418):** https://www.ncbi.nlm.nih.gov/clinvar/variation/210418/
* **UCSC Cell Browser Documentation:** https://cellbrowser.readthedocs.io/
