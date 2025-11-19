# Pan-genome analysis of 33 genetically diverse rice accessions reveals hidden genomic variations

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/ba8f6ee62080607e26ba33e747821524d5ab251430b8761832ad978c4a43476f.jpg)  
Graphical abstract

# Authors

Peng Qin, Hongwei Lu, Huilong Du, ..., Xuewei Chen, Chengzhi Liang, Shigui Li

# Correspondence

qinpeng@sicau.edu.cn (P.Q.),  
cliang@genetics.ac.cn (C.L.),  
lishigui@sicau.edu.cn (S.L.)

# In brief

A high-quality rice pan-genome of genetically diverse rice accessions is constructed through de novo genome assemblies, demonstrating the impact of structural variation and gene copy number variations on environmental adaptations and agronomic traits.

# Highlights

- De novo assembly of 31 high-quality genomes for genetically diverse accessions  
- Pan-genome-scale resources and a graph-based genome reveal hidden SVs and gCNVs  
- The derived state of O. sativa SVs was inferred using the O. glaberrima assembly  
- SVs and gCNVs have shaped gene expression profiles and agronomic trait variations

# Resource

# Pan-genome analysis of 33 genetically diverse rice accessions reveals hidden genomic variations

Peng Qin, $^{1,9,*}$  Hongwei Lu, $^{2,3,9}$  Huilong Du, $^{2,3,4,9}$  Hao Wang, $^{1,9}$  Weilan Chen, $^{1,9}$  Zhuo Chen, $^{2,3,9}$  Qiang He, $^{4}$  Shujun Ou, $^{5}$  Hongyu Zhang, $^{4}$  Xuanzhao Li, $^{4}$  Xiuxiu Li, $^{2,3}$  Yan Li, $^{2}$  Yi Liao, $^{6}$  Qiang Gao, $^{2}$  Bin Tu, $^{1}$  Hua Yuan, $^{1}$  Bingtian Ma, $^{1}$  Yuping Wang, $^{1}$  Yangwen Qian, $^{7}$  Shijun Fan, $^{1}$  Weitao Li, $^{1}$  Jing Wang, $^{1}$  Min He, $^{1}$  Junjie Yin, $^{1}$  Ting Li, $^{1}$  Ning Jiang, $^{8}$  Xuewei Chen, $^{1}$  Chengzhi Liang, $^{2,3,*}$  and Shigui Li $^{1,10,*}$  
<sup>1</sup>State Key Laboratory of Crop Gene Exploration and Utilization in Southwest China, Rice Research Institute, Sichuan Agricultural University, Chengdu, Sichuan, China  
$^{2}$ State Key Laboratory of Plant Genomics, Institute of Genetics and Developmental Biology, Innovation Academy for Seed Design, Chinese Academy of Sciences, Beijing, China  
<sup>3</sup>University of Chinese Academy of Sciences, Beijing, China  
$^{4}$ School of Life Sciences, Institute of Life Sciences and Green Development, Hebei University, Baoding, China  
$^{5}$ Department of Ecology, Evolution, and Organismal Biology, Iowa State University, Ames, IA, USA  
$^{6}$ Department of Ecology and Evolutionary Biology, University of California, Irvine, Irvine, CA, USA  
<sup>7</sup>Biogle Genome Editing Center, Changzhou, Jiangsu, China  
$^{8}$ Department of Horticulture, Michigan State University, East Lansing, MI, USA  
These authors contributed equally  
10Lead contact  
*Correspondence: qinpeng@sicau.edu.cn (P.Q.), cliang@genetics.ac.cn (C.L.), lishigui@sicau.edu.cn (S.L.) https://doi.org/10.1016/j.cell.2021.04.046

# SUMMARY

Structural variations (SVs) and gene copy number variations (gCNVs) have contributed to crop evolution, domestication, and improvement. Here, we assembled 31 high-quality genomes of genetically diverse rice accessions. Coupling with two existing assemblies, we developed pan-genome-scale genomic resources including a graph-based genome, providing access to rice genomic variations. Specifically, we discovered 171,072 SVs and 25,549 gCNVs and used an Oryza glaberrima assembly to infer the derived states of SVs in the Oryza sativa population. Our analyses of SV formation mechanisms, impacts on gene expression, and distributions among subpopulations illustrate the utility of these resources for understanding how SVs and gCNVs shaped rice environmental adaptation and domestication. Our graph-based genome enabled genome-wide association study (GWAS)-based identification of phenotype-associated genetic variations undetectable when using only SNPs and a single reference assembly. Our work provides rich population-scale resources paired with easy-to-access tools to facilitate rice breeding as well as plant functional genomics and evolutionary biology research.

# INTRODUCTION

Structural variations (SVs) are a major source of genetic variation (Weischenfeldt et al., 2013). Increasing evidence from human studies has supported that SVs are responsible for many well-known human diseases (Weischenfeldt et al., 2013), and studies in plants have implicated SVs in various phenotypes (Lye and Purugganan, 2019). Identifying SVs based on short-read sequencing data is difficult and unreliable (Sedlazeck et al., 2018). It is therefore unsurprising that SV identification based on long-read data is now becoming increasingly popular (Ho et al., 2020), such as in human (Audano et al., 2019) and plant (Alonge et al., 2020) research. This approach enables higher sensitivity and accuracy for detecting SVs short-reads. However, even with these new long-read datasets, identification of

SVs located near repeat regions, or very large SVs, remains difficult (Ho et al., 2020).

Recently, owing to advances in high-quality genome assembly, an increasing number of plant studies based on high-quality assemblies have resolved SVs among a few accessions (Hufnagel et al., 2020; Sun et al., 2018; Wang et al., 2019; Yang et al., 2019a, 2019b; Zhou et al., 2019). However, because there are few studies based on high-quality assembly at a population-scale, it is difficult to know the true extent of genomic variation in plants (Jayakodi et al., 2020; Liu et al., 2020; Song et al., 2020; Walkowiak et al., 2020), especially for gene copy number variations (gCNVs), which were recognized as an important source of functionally consequential genetic variations (Lye and Purugganan, 2019). Thus, building a pan-genome based on high-quality assemblies is desirable. One recent trend in

pan-genome studies is the construction of graph-based genomes that contain all variants in a population; these are clearly superior to conventional linear reference genomes for accurate and fast genotyping of SVs (Garrison et al., 2018; Kim et al., 2019; Liu et al., 2020; Rakocevic et al., 2019). Notably, there is a graph-based genome for the eudicot legume species soybean (Liu et al., 2020).

Rice is a major food crop for half of the global population (Wing et al., 2018) and a leading model species for monocots and crop plants in plant research. There have been several studies of SVs based on short-reads (Fuentes et al., 2019; Hu et al., 2018; Schatz et al., 2014; Wang et al., 2018; Zhao et al., 2018) as well as some population-scale and long-read sequencing data among several accessions (Zhang et al., 2016; Zhou et al., 2020). However, the extent of SVs and gCNVs, and their biological impact(s) on rice environmental adaptation and domestication, are poorly characterized. The lack of suitable SV catalogs has limited our ability to understand how SVs in plants are formed, although they are very well-studied in model mammals and humans (Carvalho and Lipski, 2016).

Here, we have de novo assembled high-quality genomes for 31 diverse rice accessions. Coupling these with two existing assemblies: Nipponbare (Kawahara et al., 2013) and R498 (Du et al., 2017), we identified a hidden legacy of genomic variation and domestication in rice. We leveraged our pan-genome-scale resources to construct a graph-based genome and inferred the derived states of SVs throughout the Oryza sativa population. We also analyzed the SV distribution and assessed the mechanisms of SV formation and SV impacts on gene expression. We provide examples of how SVs and gCNVs have directly shaped environmental adaptations and agronomic traits. Beyond showcasing the power of high-quality genome assemblies and a graph-based genome for plant genomics and functional genomics research, our study introduces a suite of resources and powerful tools to access these resources.

# RESULTS

# High-quality assemblies of 31 genetically diverse cultivated rice accessions

Cultivated rice has two species (Chen et al., 2019): Asian cultivated rice (O. sativa) and African cultivated rice (Oryza glaberrima). We selected 33 accessions, including 32 O. sativa accessions covering all known subpopulations of O. sativa and one O. glaberrima accession (Table 1). In addition to representative accessions for each rice subpopulation, we also specifically selected accessions that have greatly contributed to rice breeding and research, including popular varieties in different rice production regions of Asia (KY131, Kosh, DHX2, IR64, and WSSM), and accessions highly resistant to abiotic and biotic stress (Y3551 and N22 for heat tolerance, DG for blast resistance). The phenotypes of the 33 accessions are highly varied (Figures 1A-1D; Table S1), and a SNP analysis showed that the 33 accessions encompass fully  $89.05\%$  (minor allele frequency [MAF]  $>0.05$ ) of the SNPs present among 3,010 previously examined Asian rice accessions (Wang et al., 2018).

Two of the accessions already have high-quality genome assemblies: Nipponbare (Kawahara et al., 2013) and R498 (Du et al., 2017), and there is publicly available short-read and long-read data available for N22 (Stein et al., 2018). The 30 other accessions were sequenced at an average of  $60 \times$  depth using PacBio SMRT long-read sequencing (Table S2). Further, the 30 accessions were also sequenced to an average  $20 \times$  short-reads to facilitate correction during assembly. The 31 assemblies were de novo assembled using the CANU (Karen et al., 2017) and HERA (Du and Liang, 2019) pipelines. We ultimately generated 31 assemblies with average length of 385.8 Mbp (371.7-392.9 Mbp) for O. sativa accessions, and 344.7 Mbp for the O. glaberrima accession CG14 (Table 1). The average contig N50 length, maximum contig length, and average gap number of the 31 assemblies were 12.88 Mbp, 26.44 Mbp, and 63, respectively (Tables 1 and S2). An average of  $99.3\%$  contigs were anchored to the chromosomes (Table 1). We further evaluated the completeness of the assemblies using Benchmarking Universal Single-Copy Orthologs (BUSCO) (Simão et al., 2015), and found that an average of  $98.5\%$  ( $97.4\% - 98.9\%$ ) completeness (Table S2). Moreover, the average completeness and accuracy percentage of each assembly estimated using  $20 \times$  shortreads of each assembly were  $99.41\%$  and  $99.996\%$  (Tables 1 and S2), respectively, indicating the excellent continuity and completeness of the 31 assemblies.

Analysis using the assembly quality assessment index (LAI) (Ou et al., 2018) indicated that 30 of the assembly reached the "gold standard" level (LAI >20), whereas one (CG14) qualified at the "reference" level (Table S2). We further assessed three assemblies (02428, DG, and 9311) using BioNano map data; nearly the entire sequences (99.6%, 99.21%, and 97.30%, respectively) of all three assemblies were covered by BioNano maps, and we identified only 40, 32, and 109 InDels, respectively, between their assembly sequences and the BioNano map (Figure S1). Additionally, a total of 120 complete centromeres (no gap in centromere regions) were identified in these 31 assemblies. Collectively, all of our 31 assemblies were comparable to, or better than, the levels achieved by the rice reference genome (Nipponbare), highlighting the high quality of the new assemblies.

# Genome annotation and gene-based pan-genome construction

We identified on average 40,082 protein-coding genes for each assembly (Table 1). BUSCO evaluation (Simão et al., 2015) of the protein-coding annotations showed that an average of  $95.2\%$  of the 1,614 single copy Embryophyta genes (Table S2) were completely annotated, indicating the high completeness of the gene annotation. We further used a stepwise strategy (Zhao et al., 2018) to build a gene-based pan-genome with Nipponbare genes as the base set and obtained a pan-genome of cultivated rice comprising 66,636 protein-coding genes. Distribution analysis showed that 20,374 genes were categorized as "core genes" (i.e., present in all accessions); 46,262 genes were categorized as "variable genes" which included 14,609 accession-private genes (Figure S2A).

We also identified an average of 468,144 TEs per assembly. The average sequence length of TEs per assembly was 202.8 Mbp

Table 1. Quality assessments and annotation of 31 assemblies  

<table><tr><td>Accession</td><td>Assembly length (Mbp)</td><td>Assembly sequence accuracy (%)</td><td>Contig N50 (Mbp)</td><td>Gap number</td><td>Chromosome anchoring rate (%)</td><td>Gene number</td><td>TE number</td><td>Subpopulation</td></tr><tr><td>DHX2</td><td>376.6</td><td>99.995</td><td>6.0</td><td>120</td><td>99.5</td><td>41,060</td><td>466,341</td><td>GJ-temp</td></tr><tr><td>02428</td><td>378.9</td><td>99.997</td><td>13.5</td><td>40</td><td>99.2</td><td>39,147</td><td>466,702</td><td>GJ-temp</td></tr><tr><td>Kosh</td><td>375.2</td><td>99.997</td><td>8.9</td><td>77</td><td>99.1</td><td>40,888</td><td>465,292</td><td>GJ-temp</td></tr><tr><td>ZH11</td><td>376.8</td><td>99.997</td><td>17.3</td><td>25</td><td>99.7</td><td>37,341</td><td>465,272</td><td>GJ-temp</td></tr><tr><td>KY131</td><td>374.2</td><td>99.994</td><td>7.6</td><td>72</td><td>99.8</td><td>37,247</td><td>463,846</td><td>GJ-temp</td></tr><tr><td>NIP</td><td>373.1</td><td>N/A</td><td>7.7</td><td>62</td><td>N/A</td><td>41,096</td><td>461,226</td><td>GJ-temp</td></tr><tr><td>Lemont</td><td>379.9</td><td>99.995</td><td>6.5</td><td>128</td><td>99.3</td><td>39,479</td><td>467,214</td><td>GJ-trp</td></tr><tr><td>NamRoo</td><td>378.0</td><td>99.995</td><td>5.3</td><td>131</td><td>99.3</td><td>41,293</td><td>464,981</td><td>GJ-sbtrp</td></tr><tr><td>LJ</td><td>371.7</td><td>99.996</td><td>14.9</td><td>29</td><td>99.6</td><td>38,981</td><td>461,843</td><td>GJ-adm</td></tr><tr><td>G46</td><td>390.8</td><td>99.999</td><td>10.4</td><td>69</td><td>99.6</td><td>40,682</td><td>467,793</td><td>XI-1A</td></tr><tr><td>CN1</td><td>391.5</td><td>99.996</td><td>17.7</td><td>35</td><td>99.8</td><td>42,047</td><td>470,958</td><td>XI-1A</td></tr><tr><td>FS32</td><td>386.5</td><td>99.998</td><td>15.2</td><td>41</td><td>99.4</td><td>41,317</td><td>465,819</td><td>XI-1A</td></tr><tr><td>DG</td><td>391.1</td><td>99.994</td><td>17.0</td><td>36</td><td>99.3</td><td>41,009</td><td>467,734</td><td>XI-1A</td></tr><tr><td>D62</td><td>386.0</td><td>99.997</td><td>10.4</td><td>79</td><td>98.9</td><td>38,880</td><td>469,458</td><td>XI-1A</td></tr><tr><td>II32</td><td>389.9</td><td>99.997</td><td>13.9</td><td>40</td><td>99.6</td><td>41,887</td><td>469,544</td><td>XI-1A</td></tr><tr><td>R527</td><td>391.6</td><td>99.995</td><td>11.8</td><td>61</td><td>99.2</td><td>36,893</td><td>472,512</td><td>XI-1B</td></tr><tr><td>S548</td><td>389.5</td><td>99.995</td><td>15.2</td><td>52</td><td>99.3</td><td>43,074</td><td>469,631</td><td>XI-1B</td></tr><tr><td>9311</td><td>391.8</td><td>99.996</td><td>12.4</td><td>89</td><td>99.5</td><td>41,319</td><td>473,777</td><td>XI-1B</td></tr><tr><td>Y58S</td><td>389.0</td><td>99.996</td><td>17.7</td><td>36</td><td>99.4</td><td>42,521</td><td>471,432</td><td>XI-1B</td></tr><tr><td>J4155</td><td>388.5</td><td>99.998</td><td>9.1</td><td>82</td><td>99.1</td><td>40,137</td><td>469,773</td><td>XI-1B</td></tr><tr><td>G8</td><td>390.1</td><td>99.998</td><td>12.4</td><td>63</td><td>99.1</td><td>40,228</td><td>472,142</td><td>XI-1B</td></tr><tr><td>Y3551</td><td>390.1</td><td>99.998</td><td>10.7</td><td>73</td><td>99.2</td><td>39,913</td><td>472,490</td><td>XI-1B</td></tr><tr><td>IR64</td><td>387.6</td><td>99.995</td><td>20.9</td><td>28</td><td>99.6</td><td>39,535</td><td>466,409</td><td>XI-1B</td></tr><tr><td>R498</td><td>390.2</td><td>99.998</td><td>25.6</td><td>5</td><td>N/A</td><td>43,063</td><td>473,462</td><td>XI-1B</td></tr><tr><td>TM</td><td>390.9</td><td>99.997</td><td>23.0</td><td>34</td><td>99.4</td><td>40,082</td><td>470,826</td><td>XI-2</td></tr><tr><td>TUMBA</td><td>391.5</td><td>99.997</td><td>12.8</td><td>43</td><td>99.2</td><td>41,554</td><td>469,412</td><td>XI-3</td></tr><tr><td>G630</td><td>390.1</td><td>99.995</td><td>11.8</td><td>64</td><td>99.0</td><td>38,306</td><td>473,658</td><td>XI-adm</td></tr><tr><td>YX1</td><td>387.6</td><td>99.996</td><td>8.6</td><td>89</td><td>99.3</td><td>40,417</td><td>467,456</td><td>XI-adm</td></tr><tr><td>WSSM</td><td>390.8</td><td>99.994</td><td>7.4</td><td>141</td><td>99.6</td><td>39,193</td><td>472,251</td><td>XI-adm</td></tr><tr><td>FH838</td><td>392.9</td><td>99.998</td><td>15.1</td><td>69</td><td>99.1</td><td>37,555</td><td>476,590</td><td>XI-adm</td></tr><tr><td>N22</td><td>385.5</td><td>99.996</td><td>21.5</td><td>19</td><td>99.6</td><td>38,383</td><td>468,110</td><td>cA</td></tr><tr><td>Basmati1</td><td>380.1</td><td>99.996</td><td>9.8</td><td>56</td><td>99.3</td><td>42,098</td><td>466,659</td><td>cB</td></tr><tr><td>CG14</td><td>344.7</td><td>99.995</td><td>14.6</td><td>30</td><td>98.5</td><td>38,031</td><td>448,139</td><td>O. glaberrima</td></tr></table>

See also Tables S1 and S2.

(165.7–211.8 Mbp), accounting for an average of  $52.7\%$  (48.1%–53.9%) of the total assembly sequence length (Tables 1 and S2). Notable trends for the TEs included that the average long terminal repeat (LTR) number and the average total LTR length in the XI accessions (80,369 and 104.9 Mbp) was much higher than that in the GJ accessions (73,208 and 89.7 Mbp), this trend was led by the higher number and longer length of Gypsy LTRs in XI accessions compared to GJ accessions (59,276 versus 52,219; 90.4 Mbp versus 74.6 Mbp) (Figures S2B–S2G). Additionally, the observation of a trend that more young LTRs in XI accessions than in GJ accessions led by the higher number of young Gypsy LTRs (Figures S2H–S2J) suggested that LTRs, especially Gypsy LTRs, have undergone a relatively recent burst after the divergence of the XI and GJ rice.

# Discovery of SVs and SV hotspot regions

We compared 32 assemblies against the Nipponbare assembly using the whole-genome comparison and sequence variation annotation tool SyRI (Goel et al., 2019), with an approach that converted rearranged regions and sequence variations into three types of SVs (>50 bp): presence/absence variation (PAV), inversion, and translocation. We identified an average 24,469 (4,978 [Kosh]–34,669 [CG14]) SVs per accession relative to Nipponbare, affecting an average of 138.3 Mbp (23.4 [Kosh]–181.2 Mbp [CG14]) of genomic sequence per accession (Table S3). To check the quality of the SVs, we manually evaluated previously demonstrated SVs from the literatures and found that 12 SVs that were supposed be present in our accession panel were all present in our SVs call set (Table S3). We next

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/16bdf32b4c1a59c8e581976a0b1d77214ee7585369244939f859bcdc04548e7b.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/c836ff1e31c698919352967c840cc5202f48666d9dae9ebf4229acaac0d83dcd.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/1cb578c72178163a8a046c32d0fbb97341324b3703e2bc3da54ad082f16417f7.jpg)

Figure 1. Diverse agronomic phenotypes for genetically diverse rice accessions  
![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/d015b7493852ae5929f0bbaae7a74e481662bfb54237aa010061957c8a38d556.jpg)  
(A-D) The highly diverse agronomic phenotypes among 33 accessions, including plant height and architecture (A), grain number per panicle (B), panicle architecture (C), and grain width and length (D). These 33 accessions covered all known subpopulations of O. sativa and one O. glaberrima accessions (CG14) and encompassed  $89.05\%$  (MAF >0.05) of the SNPs present in the 3K-RG accessions.  
See also Table S1.

randomly selected 30 SVs of size ranging from 2-8 kbp and manually checked them by mapping PacBio long-reads to the genome assemblies: only one border among these SVs (1/60) differed from the borders in the mapping results (Figure S3A; Table S3). To validate large SVs, we performed Hi-C sequencing of two accessions (CG14 and TM), mapped the Hi-C paired reads to the corresponding genome assemblies, and then manually checked 30 randomly selected SVs with size ranging from 238 kbp to 5.2 Mbp at 5 kbp resolution; again, only one border among these SVs differed from the mapping results (Figure S3B; Table S3).

We next merged all SVs across accessions into a set of nonredundant SVs. In total, 171,072 non-redundant SVs affecting

1.23 Gbp of genomic sequence were cataloged, including 164,009 PAVs, 6,109 translocations, and 954 inversions. We compared the SVs in O. sativa accessions with previously identified SVs using short-reads from rice 3K-RG dataset (Fuentes et al., 2019) and found that  $82.8\%$  of PAVs in our call set have not been reported previously (Figure 2A). We also compared our SVs call set with SVs discovered using the NGMLR/Sniffles pipeline (Sedlazeck et al., 2018) with PacBio long-reads sequence data for the 32 O. sativa accessions in this study:  $67.9\%$  of our PAVs were not identified with the NGMLR/Sniffles pipeline. Notably, the missing rates for SVs obtained using both short and long-read data were positively correlated with SV size (Figure 2A). These results together suggest that the vast majority

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/edd230d2f8a00012ec9d99b88259ba080669bbe7513899ed3367dc0cdddf53f3.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/7f57bf20c9d4cde09dabc3d53ba5660b82a3355c1a36438a75aeb111bcda5f6a.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/fe13dfe300a0e07c9b4e92d8c8a6039581006fafc005c2fe8dbe10d55d1dfe1a.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/fb50279268313f5a9d037a6a707db82bd4fd9e50f1f6605d31be965eadc6e8c5.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/dcc4e3925bc21932965afde9672e7b408adebaee175b1d96a8b3183aad82040d.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/afd87290f7d685622ce2a07ee4afd8debf449511e648c0589bbfaab7249bec50.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/c5635d27d2ecdab38486889c87b2420aa4c5b4194fe834d4ef2a56aca89c7ece.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/2333f1d181216643aa973ffb400bc9774b00f63b2801a339a5a308192153554c.jpg)  
Figure 2. Inference and characterization of SVs representing a derived state

(A) Comparisons between PAVs identified in this study (excluding CG14-specific SVs) and previously identified PAVs (Fuentes et al., 2019) based on short-read data and comparisons between all PAVs in this study and PAVs identified based on the NGMLR/Sniffles pipeline with long-read data of 32 accessions. The number of “Detected” and “Undetected” PAVs, respectively, indicated the number of SVs in this study that are identified and not identified using either short or long-read datasets. Note that both these PAVs were relative to Nipponbare genome.

(B) A representative hotspot region on chromosome 11 has 868 independent SVs among the 33 accessions. Ten representative accessions are used here for displaying the positions of the SVs in this chromosome 11 hotspot region.  
(C) The number of SVs representing a derived state (dSVs) in terms of four types SV in each O. sativa accession; dSVs were inferred using the O. glaberrima accession (CG14) as an outgroup.  
(D) The frequency of dSVs in O. sativa accessions indicated most dSVs were present in one or only a few accessions  
(E) Percentage of dSVs sharing overlap with different genomic regions in 32 O. sativa accessions. Each point is one accession.  
(F-H) A region was reported to be "deleted" in XI accessions (Cardoso et al., 2014) but was actually inserted in GJ accessions based on our dSV inference (F), this inference was further supported by the distribution of this region among Oryza species (G). This region is fixed in GJ-temp and GJ-sbtrp subpopulations (H). Total number of accessions that are suitable for distribution analysis is listed after each subpopulation.

See also Figures S3 and S4 and Table S3.

of SVs cannot be identified without use of sequence comparisons with high-quality assemblies.

Our examination of SVs arrayed across chromosomes showed uneven distributions of SVs along chromosomes and re

vealed 140 SV hotspot regions (Table S3), indicating that multiple, independent SVs have arisen in these regions. Notably, one such SV hotspot region on chromosome 11 has 868 independent SVs (associated with 30 NBS family genes) (Figure 2B),

and this hotspot overlaps with (or borders) 12 blast disease resistance quantitative trait loci (QTLs) (He et al., 2014). These findings are consistent with the previously reported trend that variants positioned within SV hotspots may undergo stronger environmental selection compared to SVs positioned in other genome regions (Jiao and Schneeberger, 2020). Our delineation of SV hotspot regions can help deepen understanding about how dynamic genomic variation has contributed to responses to environmental pressures.

# Inference and characterization of SVs representing a derived state across O. sativa accessions

Because O. glaberrima and O. sativa were domesticated independently and there has been no introgression between them (Stein et al., 2018), we were able to use the O. glaberrima accession CG14 as an outgroup for an analysis inferring whether a given SV represents a derived or ancestral state. That is, for an SV having varied states among O. sativa accessions, the state that is the same as O. glaberrima CG14 is defined as the ancestral state; we termed derived-state SVs as "dSVs." A total of 130,862 dSVs (including 125,889 PAVs, 627 inversions, and 4,346 translocations) were inferred in O. sativa (Figure 2C). There were 89,981 insertions and 35,908 deletions respectively classified from these PAVs for which a derived state was inferred, so these can be assumed to reflect the evolutionary context. An obviously increased number (and larger "affected size") of insertions versus deletions was observed in the O. sativa population, as well as for each accession (Figures 2C and S4A), indicating that some evolutionary mechanism(s) have favored the emergence and/or retention of insertions over deletions. Our use of a high-quality outgroup genome assembly enabled us to confidently infer the derived state of large SVs. For example, we can now see that the Nipponbare sequence of a previously reported inversion on chromosome 6 between Nipponbare and R498 (Du et al., 2017) actually represents the derived state because most O. sativa accessions and CG14 share the same state (Figures S4B and S4C).

Analysis of the dSV distribution in terms of size revealed that  $60.6\%$  (79,355) of SVs were between 50 bp-2 kbp,  $22.6\%$  (29,622) were between 2 kbp-10 kbp, and  $16.7\%$  (21,881) were  $>10$  kbp (Figures S4D and S4E). The frequency of dSVs in O. sativa accessions showed that most dSVs were present in one or only a few accessions (Figure 2D). We further analyzed the dSV distribution in terms of relative position to genes and found that  $53.2\%$  of dSVs overlapped with genic regions (including coding regions, introns, and  $\pm 2$  kbp of coding regions) (Figure 2E) across 32 O. sativa accessions. A majority of dSVs associated with genic regions shared overlap with the sequences  $\pm 2$  kbp of coding regions (Figure 2E). The frequency of dSVs overlapping with coding regions was obviously lower than the derived alleles of SNPs located in coding regions (Figure S4F). We found that  $\sim 50\%$  (32,668) of the genes in the pan-genome had at least one dSV overlapped with their genic region (henceforth termed "dSV-genes") across the 32 O. sativa accessions, and  $52.6\%$  (1,406) of all functionally studied rice genes (http://funricegenes.ncpgr.cn/; Yao et al., 2018) have a dSV in at least one of these accessions, including previously reported dSV-genes that have contributed to environmental

adaptation like OsTPP7 (Kretzschmar et al., 2015) and to human selection like SD1 (Sasaki et al., 2002).

The inference of dSVs can help to understand the direction and biological significance of natural and/or artificial selection acting on SVs. For example, a region harboring the  $SLB1$  and  $SLB2$  loci was reported to be "deleted" in XI accessions (Cardoso et al., 2014), and the "deletion" of this region was associated with higher tiller number and reduced strigolactone (SL) production (thus reducing the seed germination of parasitic Strigas) (Cardoso et al., 2014). However, our inference of SV ancestral state showed that this region was very likely inserted into GJ accessions (Figure 2F), because CG14 and almost all XI accessions shared the same state for this region; this insertion in GJ accessions was also supported by the absence of this region (inferred based on the mapping coverage ratio) in other Oryza species from a previous study (Stein et al., 2018; Figure 2G). Further, the distribution based on SV sequence coverage by short-reads in the 3K-RG dataset (Wang et al., 2018) and 13 wild rice accessions (Zhao et al., 2018) showed that this insertion was nearly fixed in the GJ-temp and GJ-sbtrp (temperate and subtropical Geng/Japonica) subpopulations (Figure 2H), indicating it had been selected during the GJ domestication process.

Overexpression of  $SLB1$  increased SL content (Cardoso et al., 2014), and SL can enable rice to acquire more phosphorus (Xie et al., 2010) by inducing hyphal branching of arbuscular mycorrhizal fungi (Akiyama et al., 2005). Moreover, the expression of  $SLB1$  was shown to be significantly increased under phosphorus deficiency (Figure S4G; Xia et al., 2017). It is therefore possible that this insertion harboring  $SLB1$  was selected because it could enable rice to acquire more phosphorus under low phosphorus conditions and thereby increase rice productivity. These data illustrate how large-scale inference of dSVs in O. sativa and our dSV-gene catalog can support investigations into rice evolution and domestication.

# SVs have broadly shaped gene expression profiles

SVs have been reported to influence the expression of nearby genes by altering gene sequences or by affecting regulatory sequences (Alonge et al., 2020; Liu et al., 2020), and our data indicated that a majority of dSVs overlapped with non-coding regions (Figure 2E). We therefore explored the general expression characterization of dSV-genes using RNA sequencing (RNA-seq) data for 29 diverse sample types from the R527 accession (including leaf, panicle, stem, and caryopsis at different stages, as well as shoots and roots treated with different abiotic stress conditions) (Table S4). We first compared the fold changes in the expression levels for both dSV-genes and nonSV-genes of R527 between pairwise samples for which only one stress condition differed (mechanical pressure, temperature, hypoxia, or osmotic stress) (Figure S5A; Table S4); note that "nonSV-genes" here refers to genes with a genic region lacking overlap with any SV. In each of the 12 pairwise samples, the proportion of dSV-genes having a  $>3$ -fold expression changes after stress treatment was obviously higher than the proportion of nonSV-genes (Figures 3A and S5B). This suggests that the dSV-genes are generally more sensitive to these environmental stresses.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/acc30b604f0fe78c8527922e0fc6bb9c2493b7681bb8e4274c78462cc268ae38.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/76a5cc1e75bd4a90237b05412a40dd2bbb8b9959152f8039aa650104adf46272.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/ad3861584692cfc43271684b0ad22a211eb17598438cda1a974a0faff41832cb.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/0229b3defaef97d42eb084db3e9a86cf0c600c4277e94d4e2409dcbe1a53f5f7.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/6f1bd591747184cc33bcb59277c672271650aa0578970f632f35069e4737fa3a.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/422c4a716cde1c081bde8b8bc5a1502bfb539805c785638d04c78f2cdb304d60.jpg)

Figure 3. Impacts of SVs on genes have shaped environmental adaptation and domestication  
![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/02ffeecdaafba1319b1e8e1e762b6cdbef3af59036883347dae1e3a3090959b9.jpg)  
(A) Proportion comparisons between dSV-genes and nonSV-genes with different expression fold change after only one indicated stress treatment. All samples, dSV-genes, and nonSV-genes are from R527 accession. See also Figure S5A and Table S4 for treatment details.  
(B) Proportion comparisons between dSV-genes and nonSV-genes with indicated expression level across 29 samples from R527 (including leaf, panicle, stem, and caryopsis at different stages, as well as 16 samples including seedling root or shoot for stress treatments).

When expanding to all 29 of the sample types, there were three additional clear trends in the expression levels of dSV-genes compared to the nonSV-genes: the dSV-genes generally tended to be expressed in fewer of these tissues and conditions (Figure S5C); the proportion of "low expression" genes was invariably higher among the dSV-genes in all sample types (Figure 3B); and the expression level for the whole set dSV-genes were significantly lower than for the nonSV-gene set across the 29 sample types (Figure S5D). These trends all support the idea that, generally speaking, genes directly impacted by dSVs tend to have relatively low expression levels and are apparently more sensitive to environmental stress.

To investigate the potential impacts of dSVs on the expression of particular genes, we performed RNA-seq of root and shoot materials for the 33 accessions. The presence of  $15.6\%$  (3,340) of the SVs (present in  $>3$  yet  $<29$  accessions) sharing overlap with a genic region was associated  $(p < 0.05$  and  $|r| > 0.5)$  with altered expression of their corresponding genes in roots and/or shoots. Specifically, 1,433, 438, 416, and 1,176 dSVs, respectively, overlapped the upstream, coding region, intron, and downstream sequences significantly associated with altered expression of corresponding genes in root and/or shoot materials (Figures 3C and S5E; Table S5). These analyses collectively indicate that SVs have broadly shaped gene expression profiles during rice evolution and domestication.

# Contribution of SVs in rice environmental adaptation and domestication

Coupled with our dSV distribution analysis that revealed thousands of subpopulation-specific dSVs (Figure S5F), our catalog of dSV-gene and aforementioned analyses of gene expression should be helpful for discovering the underlying genetic basis of environmental and human selection. For example, these datasets can support straightforward population-scale confirmatory analysis about specific functional impact(s) from dSVs in an accession of interest or supporting hypothesis generation about how particular dSV-genes have influenced a trait-of-interest in a particular subgroup of rice accessions. To augment the utility of this catalog of dSV and dSV-genes, we further analyzed the distribution of dSVs in a greater population based on the coverage ratio of SV sequences from short-read data. This analysis included 3,010 O. sativa (Wang et al., 2018) and 13 wild rice accessions (Zhao et al., 2018), all of which were mapped to the Nipponbare genome to infer whether an SV sequence was present (coverage ratio  $>75\%$ ) or absent (coverage ratio  $>25\%$ ) in a given accession.

Note that this approach limited our investigation to the distribution of SVs for which either the ancestral or derived sequence is present in the Nipponbare genome. This approach revealed the distribution of 20,965 dSVs from the dSV catalog, including 17,378 deletions and 3,587 insertions (Table S5). Specifically, there were 5,393 (25.7%) dSVs that were fixed (present in all accessions of a given subpopulation) in one or more subpopulation (Figure 3D). We found that 2,535 fixed dSVs were present in a single subpopulation, and 799 fixed dSVs were present in more than 5 (>50%) subpopulations (Figure S5G; Table S5). Besides fixed SVs in O. sativa, we also found 1,261 dSVs that were present in all 13 of the examined wild rice accessions (Figure 3D; Table S5).

Our findings based on this Nipponbare-centric approach of  $25.7\%$  fixed dSVs among the 20,965 examined dSVs suggests that many more fixed dSVs are likely present in our dSV catalog; deconvoluting these will be helpful for studying underlying environmental adaptation and/or human selection during rice evolution and domestication. For example: an insertion at 643 bp upstream of OsGLP2-1 was found in 8 out of 9 GJ accessions of this study, and this insertion was associated with increased expression in GJ accessions (Figure 3E and 3F). As compared to its frequency in wild rice accessions, this insertion has become nearly or completely fixed among the GJ, circum-Basmati (cB), and circum-Aus (cA) subpopulations (Figure 3H). Given that knockdown of OsGLP2-1 in the GJ background was shown to block seed dormancy and its overexpression was shown to strongly increase seed dormancy (Wang et al., 2020), it appears that the expression level of OsGLP2-1 can help ensure appropriate seed dormancy in the GJ background. Accordingly, this insertion in the GJ accessions may have been selected during the domestication of GJ, cA, and cB rice. This speculation is also supported by a seed dormancy QTL containing OsGLP2-1 previously identified from the XI/GJ population (Yuan et al., 2020).

We also found two independent dSVs (a 66.6 kbp deletion in one GJ accession and a 43.3 kbp deletion in one cA, one cB, and three XI accessions) (Figure 3G); these dSV regions each contained the full sequence for a known negative regulator gene for blast resistance, OsWAK112d (Delteil et al., 2016). Apparently, both of these independent deletions have contributed to environmental adaptation by enhancing blast disease resistance. Further analysis of the distribution of OsWAK112d in the 3K-RG panel dataset showed that OsWAK112d is present in at least  $85\%$  of the accessions comprising the cA, XI-1A, XI-1B, and XI-2 subpopulations (Figure 3H), suggesting that its

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/2e84f2e0918b51436d793af2800e4c7b79f7d531886f3f9a8f3aea2c7af3c59b.jpg)  
A  
B

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/f22f03455640d6aa5518ef2676f523f6a556081891f866103e0323354ca647f9.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/e6febca7728a25fd8aee2046d927ac9f081796ada6b5f2287bcd533534ffceff.jpg)  
C

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/85394c613baf418fae725a5f3e234000b4a90f0b67717702049e688995efcae4.jpg)  
D  
F

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/a5bf26bce88fd0f8b47dde923bcc31c05b575ae28b16c080bb92e9c75c91b503.jpg)  
G

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/97456803a3dc1531211f4e831c478f1b3d495b34e95cbb45b468fa69e765ed8d.jpg)  
E

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/c604b44ec1f9971293eed12927c7284136559d9a114c494c19864723049c6d5f.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/b8d5939cb409c74a116e41685d683e77c9b9a29716526ac432e81eb107378def.jpg)  
J

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/b27fbcbe984a40ecad04fa2602a256040db8b9100de9e90884ec17a7a92e6066.jpg)  
H

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/a545fe71e203d768e290dc9d3bb79f22586b358c1cf870fb44586376ea49e5fa.jpg)  
1

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/dfcc751aad737ba1105b5480c05de9e0eed89ff3fa013d9b6e057fbab4943bd2.jpg)  
L

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/080b563255f52b6185377b98a2c73d2881d8bad58e50e21989d6b5210f2c374a.jpg)  
M  
N

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/14054da3a43d3163f0c829d10c81bdd3a5e42525967e05d0d04b83f9ccb606d2.jpg)  
  
K

0  
Figure 4. Gene CNVs are widespread and are associated with agronomic trait variation  
![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/95f6ab68412cc879e950cf03c9919db4cb25877d06dd31f64f0ed6a061db7621.jpg)  
(A) The number and percentage of pan-genome genes with or without CNVs across the 33 assemblies. *If two or more genes in the pan-genome shared both identity and coverage >90%, we only selected one gene for CNV identification, the remaining genes are not used for CNV identification.

deletion may have increased the rice blast resistance of these accessions. Beyond dSV-genes, there were 3,699 additional genes sharing overlap with SVs for which a derived state could not be confidently inferred. Thus, given previous studies in rice showing that SVs located beyond  $\pm 2$  kbp of a coding region can also function in regulating gene expression (Duan et al., 2017; Liu et al., 2017), it can be confidently assumed that the extent of contributions to environmental adaptation and domestication from SVs actually extends well-beyond this initial catalog of dSV-genes from our study.

# Gene CNVs are widespread and are associated with variations in agronomic traits

It is now clear that gCNVs have contributed widely to crop evolution and domestication; however, resolving gCNVs remains challenging (Lye and Purugganan, 2019). We took advantage of our high-quality assemblies and systematically explored gCNVs by harnessing an unbiased alignment of predicted protein sequences for pan-genome genes against the 33 assemblies. In total, gCNVs were inferred for 25,549 (38.34%) of the protein-coding genes in the rice pan-genome (Figure 4A), including 2,945 inferred as CG14-specific gCNVs and 22,604 inferred as gCNVs in O. sativa (Figure 4A), a notably higher level than reported in a previous genome-scale study in rice (1,321 CNV genes) (Yu et al., 2013). We noted that the catalog of gCNVs included 14,782 gene PAVs. Among the gCNVs, we found the previously reported two copies of GL7 (Wang et al., 2015) and Sc (Shen et al., 2017), and 320 additional functionally investigated genes that have not been previously reported as having any CNVs in rice, such as a blast resistance gene (Pid4) (Chen et al., 2018) and a drought tolerance gene (OsDT11) (Li et al., 2017). Moreover, the expression level of 296 and 361 genes (without gene PAV) were correlated  $(p < 0.05$  and  $|r| > 0.5)$  with CNVs in shoots and roots, respectively (Figure 4B; Table S6), indicating that a large number of potentially functional gCNVs have been previously neglected.

For example, seven O. sativa accessions harbor two copies of OsVIL1 that are positioned  $\sim 193$  kbp apart on chromosome 8 (Figures 4C and 4D) and we found that the expression level of OsVIL1 in these accessions (i.e., harboring two copies) was significantly higher than the level in accessions harboring a single copy (Figures 4E and 4F). Given that increased OsVIL1 expression causes rice to flower early in short-day conditions but causes delayed flowering and increased grain number in long-

day conditions (Jeong et al., 2016), the CNV of OsVIL1 is likely associated with flowering time and grain number variation. The duplication of OsVIL1 could potentially confer increased grain number in long-day conditions. Additionally, inference of two OsVIL1 copies using resequencing data from the 3K-RG dataset (Wang et al., 2018) and wild rice accessions (Zhao et al., 2018) (based on reads depth) revealed an apparently elevated frequency of the inferred two OsVIL1 copies in the cA and XI-1B subpopulations compared to wild rice (Figure 4G), indicating potential selection for the extra copy of OsVIL1 in these O. sativa accessions.

Beyond the impacts on increasing expression, gCNVs can also lead to ectopic expression patterns (e.g., when the promoter region of the extra copy is different from its parent copy). We found that two copies of Kala4 were identified in N22, and close examination found that one border of the duplicated DNA fragment (harboring the entire Kala4 gene) was close to the Kala4 start codon, yielding a distinct promoter sequence for the derived copy from the parent Kala4 copy (Figure 4H and 4I). Given that activated Kala4 expression in pericarp specifically activates the genes in the anthocyanin biosynthesis pathway (causing a "black pericarp" phenotype) (Oikawa et al., 2015), and considering that N22 is the only accession we examined that has a black spikelet top (Figure 4J), it seems plausible that Kala4 may be ectopically expressed in the top of N22 spikelets. Indeed, we performed an expression analysis of spikelets from Nipponbare and N22 accessions and found that Kala4 expression was only detected in the top of N22 spikelets (Figure 4K), supporting that the ectopic expression of the extra Kala4 copy can very likely account for the black spikelet top phenotype of N22.

This gCNV catalog was also helpful for confidently pinpointing candidate variants responsible for phenotypic variation of QTLs located in complex regions. For example, we found that Koshihikari specifically harbored a tandem duplication of OsMADS18. The dual copies of OsMADS18 were located in a tandem repeat sequence in Koshihikari (Figures 4L and 4M) and these were associated with elevated OsMADS18 expression (Figure 4N). We found that OsMADS18 is located in the previously reported early flowering QTL (qDTH7-3) in Koshihikari that was mapped using a population derived from a Koshihikari  $\times$  IR64 cross (Nonoue et al., 2019). Considering that increased expression of OsMADS18 has been shown to result in early flowering (Qu et al., 2006; Yin et al., 2019), we can infer that the duplication

of OsMADS18 is a likely causal candidate accounting for this early flowering QTL.

This early flowering QTL associated with OsMADS18 duplication may have helped shape the early flowering properties underlying the wide geographic adaptability of the famous Koshihikari accession (Kobayashi et al., 2018). An inference of two OsMADS18 copies in the 3K-RG dataset (Wang et al., 2018) and wild rice accessions (Zhao et al., 2018) (based on reads depth) revealed that only two GJ-temp accessions have two OsMADS18 copies (Figure 4O), indicating that this OsMADS18 duplication has not yet been widely applied, so it should be useful in rice breeding. Collectively, this catalog of gCNVs is helpful for investigating potentially hidden genomic variation underlying phenotypic variations in rice.

# Diverse mechanisms drive SV formation in rice

Seeking to better understand the driving forces and specific mechanisms that have contributed to SV formation, we employed a workflow (Kidd et al., 2010; Yang et al., 2013) based on characterization of the breakpoint sequences for the dSVs in O. sativa accessions (Figures 5A, S6A, and S6B). Overall,  $48.7\%$  derived alleles of SVs were confidently assigned a particular formation mechanism. The dominant formation mechanism among these assigned SVs was transposable element insertion (TEI)  $(50.8\%)$ , followed by nonhomologous end joining (NHEJ)  $(43.9\%)$  (Figure 5B; Carvalho and Lupski, 2016). This is different from the dominant mechanism in genomes of human cancer patients, where NHEJ and alternative end jointing predominate (Yang et al., 2013). Beyond these dominant mechanisms in rice, our analysis showed that 2,741 dSVs were formed through the fork stalling and template switching/microhomology-mediated break-induced replication (FoSTeS/MMBIR) mechanism (Figure 5B; Carvalho and Lupski, 2016).

We also conducted a closer examination that revealed that the dominant mechanism was variable among different types of SV. For example, most deletion (70.1%) and translocation (83.7%) SVs were formed by NHEJ, whereas a majority (93.8%) of insertion SVs were formed via TEI (Figure 5C). This also revealed that inversion SVs were mainly formed by FoSTeS/MMBIR (54.9%), followed (in ranked order) by NHEJ (29%) and non-allelic homologous recombination (NAHR) (16%) (Figure 5C). Beyond SV type, our analysis based on SV size showed that more than half SVs shorter than 5 kbp were formed by TEI, whereas those longer than 5 kbp resulted mainly from NHEJ. Notably, over 25% of very large SVs (>100 kbp) were formed by FoSTeS/MMBIR (Figure 5D).

Examination of the subset of rice SVs formed by TEI indicated that  $55\%$  and  $38.3\%$  were from DNA TEs and LTRs, respectively (Figure 5E). We next analyzed the potential roles of TEs in the set of SVs that were apparently formed through two major non-TEI mechanisms (NHEJ and NAHR), specifically by characterizing TEs at SV borders. Overall,  $73.2\%$  of the SVs borders formed by NHEJ and NAHR overlapped with TEs, and this proportion varied among SV types (from a high of  $87.2\%$  for translocations to a low of  $53.1\%$  for inversions) (Figure S6C). A close examination showed that  $73.2\%$  of SVs formed by NHEJ and  $81\%$  of SVs formed by NAHR had at least one breakpoint which overlapped with a TE. Additionally, the TEs that overlapped with SV borders

formed by NHEJ and NAHR had a higher LTR proportion (31.7% and 54.5%, respectively) compared to the value for the whole genome (16.6%) (Figure 5E). Collectively, these results indicate that TEs, and especially LTRs, are able to somehow frequently generate DNA breaks for NHEJ or to facilitate NAHR by providing homologous sequences.

# Building and exploring the utility of a graph-based genome in rice

By taking advantage of a variation graph toolkit (Garrison et al., 2018), we built a graph-based genome using PAV sequences sharing  $<50\%$  identity with each other and using the Nipponbare genome as the base linear genome. A total of 66,542 PAVs were integrated into the graph-based genome. The assessment indices for this graph-based genome (recall:  $81.9\%$ , precision:  $83.6\%$ , and  $F_{1}$  score: 0.827) were comparable to previous values reported for soybean and yeast (Hickey et al., 2020; Liu et al., 2020). To help demonstrate the utility of the graph-based rice genome, we selected the resequencing short-reads of 674 accessions (sequencing depths  $>10x$ ) from the rice 3K-RG dataset (Wang et al., 2018) equably covering all subpopulations of O. sativa rice (Table S7) and then mapped them to the graph-based genome. In total, we identified 47,952 PAVs including 7,862 newly identified PAVs. These PAVs were enriched  $(63\%)$  in those of size  $<500$  bp, and there were also 2,417 PAVs  $>10$  kbp (Figure S7A). Our finding that the distribution pattern of these PAVs (in terms of subpopulations) was similar to the pattern for the PAVs identified relative to Nipponbare among the 32 O. sativa accessions (Figure S7B) suggests no obvious subpopulation biases for the PAVs from the graph-based genome. We further investigated how frequently the SVs from 674 accessions (MAF  $>2\%$ ) were linked to nearby SNPs, seeking to determine the extent of previously uncovered genetic variations:  $17.5\%$  of SVs showed very low linkage with nearby SNPs  $(r^{2} < 0.25)$  (Figure 6A), indicating the presence of a hidden genetic variation that cannot be represented by SNPs.

We also performed a genome-wide association study (GWAS) for leaf senescence phenotypic data of these 674 accessions (https://snp-seek.irri.org; Table S7) using both their SNPs (Wang et al., 2018) and SVs based on the graph-based genome. A locus harboring two SVs was significantly associated with early leaf senescence on chromosome 6 that was not identified based on SNP data (Figure 6B). The most strongly associated SV was a 987-bp LTR insertion positioned 230 bp upstream of the Os06 g13470 locus (encoding a predicted S-adenosyl-L-methionine dependent carboxyl methyltransferase) (Figure 6B), and was present in 18/674 accessions, a majority of which (16) belong to the XI-1A subpopulation (Figure S7C). A follow-up expression analysis showed that this insertion was specifically linked with the activated expression of Os06 g13470 in Y3551 (the single accession harboring this insertion among the 33 accessions in the present study) during leaf senescence (Figure 6C), further supporting that this insertion likely contributes to variation in leaf senescence. These results illustrate how our graph-based genome can support re-analysis of previously reported short-read data for rice, thereby extending the application prospects of such datasets for advancing rice functional genomics research.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/70f2a032fe76911996cb247a8c92fdc8470b1f5307a033cee94a2e3ac1561c8c.jpg)  
A

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/7efb9a492e821453d5d187caf69a94c149aad36277963db8ca813809945c34b2.jpg)  
B

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/1e348c619dd259408979cf7581b882330b3360cfef58b8943066ee767cb79e1f.jpg)  
C

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/cb5a646c8fdc3de84b62466b335f9e07250f5f2dc4c95d49302a43187b367b40.jpg)  
D  
Figure 5. Diverse mechanisms drive SVs formation in rice

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/07cfbe4cc712e5af4cb42e8e40598e37acefef4d4e7ff1fa88035435cff74ab4.jpg)  
E

(A) Flowchart showing the breakpoint features for assigning mechanisms of insertion or deletion, the flowchart is based on Yang et al. (2013). TEI, transposable element insertion; VNTR, variable number of tandem repeats; NHEJ, nonhomologous end joining; alt-EJ, alternative end joining, SSA, single strand annealing; NAHR, nonallelic homologous recombination; FoSTeS/MMBIR, fork stalling and template switching/microhomology-mediated break induced repair. *Both deletions and insertions are assigned the FoSTeS/MMBIR mechanism.

(B) The proportion of SVs formed by each of the seven examined mechanisms in rice.  
(C) The proportion of different mechanisms in terms of four SV types, highlighting that the dominant mechanism differs among the SV types.  
(D) The percentage of SVs formed by different mechanisms in terms of SV size.  
(E) The proportions comparison of four TE types among all TEs (i.e., genome-wide), TEs that formed SVs through the TEI mechanism, and TEs that overlap with the breakpoints of SVs formed by the NHEJ or NAHR mechanisms.

See also Figure S6.

# A web-based tool provides easy access to these genomic resources

To facilitate ready-access to these resources, we have developed a web-based tool (http://www.RiceRC.com). Researchers can quickly determine whether there are any SV or CNVs for any

gene-of-interest (or at any genome position). The tool integrates a genome browser and a BLAST function, which allows researchers to launch various analyses using all of the high-quality assembly sequences. This web-based tool also contains a comprehensive catalog of SNPs/Indels, including the SNP/

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/11644b2334da092115590d0407be8b2681ae8ccd1ae2ffef658ce32ff308eb33.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/def15656a9aa662418c7b3f9b56e909cb9b68373090e0f7ef1c76d62e1e7eacf.jpg)  
(B) GWAS for leaf senescence phenotypes (from https://www.snp-seek.irri.org) using SVs based on graph-based genome and previously characterized SNPs from the 674 accessions from the rice 3K-RGP dataset. A locus on chromosome 6, which was identified using SVs but not SNPs, was significantly associated with early leaf senescence. The most strongly associated SV was a 987 bp LTR insertion at the promoter of Os06 g13470.

Figure 6. Building and demonstrating the utility of a graph-based genome in rice  
![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/11695eceaff98f0ca4cdfaebb38d21b2d54dbb31f24d8f5220e9ed2c4787939f.jpg)  
(A) Linkage analysis between SVs from the graph-based genome using 674 accessions from the rice 3K-RG resequencing panel (Wang et al., 2018), and their nearby  $(\pm 500\mathrm{kbp})$  SNPs.  
(C) Expression analysis of Os06 g13470 in leaves at four different developmental stages in five accessions. Y3551 was the only accession that harbors this LTR insertion among the 33 accessions.

See also Figure S7 and Tables S4 and S7.

Indels that were previously filtered out (or could not be detected) because of highly repetitive or non-Nipponbare sequences in previous SNP call sets. It also includes the ancestral allele data for these SNP/Indels, which can benefit the crop research and breeding communities.

# DISCUSSION

Rice is a staple crop that feeds billions of people globally. Obtaining a deeper understanding of hidden genomic variation legacy of rice evolution and domestication can significantly benefit agriculture and world food security, as well as the biological and genomic research communities. In the present study, we took advantage of two existing and 31 new high-quality assemblies of diverse accessions to generate a pan-genome dataset in rice. Importantly, we have employed these datasets to infer SVs representing the derived state, and analyzed their distributions in O. sativa accessions. Given that knowing the ancestral/derived state of each SV can support inferences about the evolutionary relationships and the genetic basis of phenotypic diversity in the rice population, these rich dSV datasets and our dSV-gene catalog represent useful tools for investigations of rice evolution and domestication history and for hypothesis generation in functional genomics studies.

Beyond the representative pan-genome resources we present, our study also offers illustrative examples of how these resources can deepen our understanding of how SVs and gCNVs

have contributed to environmental adaptation and artificial selection in rice evolution, domestication, and expansion processes. Our datasets enabled exploration of SV formation mechanisms in rice, which establishes a foundational dataset for such analyses in monocot crop species. If similar analyses are conducted for other plant species, then interspecies comparisons about SV formation mechanisms will be possible. Such analyses could for example uncover how major events from evolutionary history—for instance the activation of genus-specific repetitive elements—have differentially impacted SV formation among diverse plant lineages. Additionally, we noted that nearly  $80\%$  of gCNVs were not correlated with expression changes (Figure 4B); this may indicate that some additional copies have been quickly silenced—that would mirror reports about repression of transcription of newly duplicate genes based on DNA methylation in Arabidopsis (Wang et al., 2016)—or might indicate that the overall expression level of a gene (transcribed from all copies) has been reduced after CNVs have occurred.

Additionally, our reference-quality genomes will be helpful to the very large number of research groups doing various basic biological studies, such as designing genomic edits and promoting successful mapping of causal mutations positioned within highly complex and/or duplicated regions. The graph-based genome also offers a platform that enables researchers to obtain substantially more information than a single reference genome for other sequencing-based analyses such as chromatin immunoprecipitation sequencing (ChIP-seq) and RNA-seq (Garrison

et al., 2018; Kim et al., 2019; Rakocevic et al., 2019). The resources presented in the present study can greatly benefit the crop improvement and plant research communities.

# Limitations of study

Although our study provides a pan-genome-scale resource, several limitations should be mentioned. First, our manual validation of SVs indicated a number of SVs have borders that do not exactly match their positions in the present genome assemblies. Additionally, the accuracy of inferences about SV ancestry states will be improved as emerging studies report additional high-quality assemblies from wild species of the Oryza genus. Assigning SV formation mechanisms based on the breakpoint sequence features of dSVs is still an inexact process. For instance, there is no consensus cutoff for the homologous sequence length between alt-EJ and NHEJ mechanisms. Another issue is that the gene copies identified in each assembly using our strategy could have acquired novel functions or become non-functional, depending on how the copied protein coding and/or regulatory element region(s) were generated and on how they have been subsequently influenced by yet-further mutations (e.g., SNP/Indels); the number of such cases is not yet clear. Finally, given the 66,542 SVs integrated into the graph-based genome, yet considering that our short-read data analysis from 674 accessions genotyped 47,952 SVs, many SVs were not successfully identified using this approach. We anticipate that further population-scale, long-read sequencing datasets, as well as improvements in both mapping and variant-calling algorithms, will help overcome this limitation.

# STAR\*METHODS

Detailed methods are provided in the online version of this paper and include the following:

- KEY RESOURCES TABLE  
- RESOURCE AVAILABILITY

Lead contact  
Materials availability  
$\bigcirc$  Data and code availability

- EXPERIMENTAL MODEL AND SUBJECT DETAILS  
$\bullet$  METHOD DETAILS

$\bigcirc$  Investigation of agronomic traits  
$\bigcirc$  Preparation of short-read sequencing libraries  
$\bigcirc$  RNA sequencing and data analysis  
Long-reads sequencing and de novo genome assembly  
$\bigcirc$  Short-reads data processing  
Construction of BioNano optical maps  
$\bigcirc$  Population structure analysis  
○ Gene annotations  
Repeat sequence annotation  
Estimation of TE duplication times  
$\bigcirc$  Gene-based pan-genome construction  
$\bigcirc$  SV identification  
SV validation  
SV comparisons  
Identification of SV hotspot regions

$\bigcirc$  Merging SV and inferring the derived SVs  
Distribution of SVs relative to gene position  
Identification of gene CNVs  
$\bigcirc$  Inference of CNVs using short-read data  
Experimental analysis of gCNV and expression level  
$\bigcirc$  SV formation mechanisms  
$\bigcirc$  Graph-based genome construction

QUANTIFICATION AND STATISTICAL ANALYSIS

# SUPPLEMENTAL INFORMATION

Supplemental information can be found online at https://doi.org/10.1016/j.cell.2021.04.046.

# ACKNOWLEDGMENTS

We thank all the members of the Shigui Li group at Sichuan Agricultural University and the Chengzhi Liang group at the Institute of Genetics and Developmental Biology of the Chinese Academy of Sciences for helpful discussions. We thank Dr. Lixing Yang at the University of Chicago for helpful discussions about SV formation mechanisms. We thank Dr. Sheila McCormick at UC Berkeley and Dr. John Hugh Snyder at the National Institute of Biological Sciences, Beijing for editing. This work was supported by the National Key Research and Development Program of China (2016YFD0100400), Chinese Academy of Sciences "Strategic Priority Research Program" (XDA24040201), the National Natural Science Foundation of China (92035301), and State Key Laboratory of Plant Genomics.

# AUTHOR CONTRIBUTIONS

P.Q., H.L., H.D., H.W., W.C., and Z.C. contributed equally to this study. P.Q., H.L., W.C., H.Z., and Xuanzhao Li conducted the SV and CNV identification and the SV mechanism analysis. H.D., Q.H., and H.Z. conducted genome assembly and quality assessments and built the graph-based genome. Z.C conducted the GWAS and linkage analyses. W.C., T.L., B.T., and H.W. conducted the phenotypic analysis. H.W., H.Y., and S.F. collected samples for RNA-seq sequencing and conducted expression validation. Y.W., Y.Q., and B.M. developed the web-based analytical tools. S.O. and N.J. worked on TE annotation. Yi Lao annotated centromeres. Z.C., Xiuxiu Li, Yan Li, and Q.G. annotated protein coding genes. W.L., J.W., M.H., J.Y., and X.C. analyzed data. P.Q., C.L., and S.L. wrote the manuscript, designed, and supervised this project.

# DECLARATION OF INTERESTS

The authors declare no competing interests.

Received: January 10, 2020

Revised: January 31, 2021

Accepted: April 24, 2021

Published: May 28, 2021

# REFERENCES

Akiyama, K., Matsuzaki, K., and Hayashi, H. (2005). Plant sesquiterpenes induce hyphal branching in arbuscular mycorrhizal fungi. Nature 435, 824-827. Alexander, D.H., November, J., and Lange, K. (2009). Fast model-based estimation of ancestry in unrelated individuals. Genome Res. 19, 1655-1664.

Alonge, M., Wang, X., Benoit, M., Soyk, S., Pereira, L., Zhang, L., Suresh, H., Ramakrishnan, S., Maumus, F., Ciren, D., et al. (2020). Major Impacts of Widespread Structural Variation on Gene Expression and Crop Improvement in Tomato. Cell 182, 145-161.e23.

Audano, P.A., Sulovari, A., Graves-Lindsay, T.A., Cantsilieris, S., Sorensen, M., Welch, A.E., Dougherty, M.L., Nelson, B.J., Shah, A., Dutcher, S.K., et al. (2019). Characterizing the Major Structural Variant Alleles of the Human Genome. Cell 176, 663-675.e19.

Cardoso, C., Zhang, Y., Jamil, M., Hepworth, J., Charnikhova, T., Dimkpa, S.O., Meharg, C., Wright, M.H., Liu, J., Meng, X., et al. (2014). Natural variation of rice strigolactone biosynthesis is associated with the deletion of two MAX1 orthologs. Proc. Natl. Acad. Sci. USA 111, 2379-2384.  
Carvalho, C.M., and Lipski, J.R. (2016). Mechanisms underlying structural variant formation in genomic disorders. Nat. Rev. Genet. 17, 224-238.  
Chen, Z., Zhao, W., Zhu, X., Zou, C., Yin, J., Chern, M., Zhou, X., Ying, H., Jiang, X., Li, Y., et al. (2018). Identification and characterization of rice blast resistance gene Pid4 by a combination of transcriptomic profiling and genome analysis. J. Genet. Genomics 45, 663-672.  
Chen, E., Huang, X., Tian, Z., Wing, R.A., and Han, B. (2019). The Genomics of Oryza Species Provides Insights into Rice Domestication and Heterosis. Annu. Rev. Plant Biol. 70, 639-665.  
Chen, Z., Li, X., Lu, H., Gao, Q., Du, H., Peng, H., Qin, P., and Liang, C. (2020). Genomic atlases of introgression and differentiation reveal breeding footprints in Chinese cultivated rice. J. Genet. Genomics 47, 637-649.  
Delteil, A., Gobbato, E., Cayrol, B., Estevan, J., Michel-Romiti, C., Dievart, A., Kroj, T., and Morel, J.B. (2016). Several wall-associated kinases participate positively and negatively in basal defense against rice blast fungus. BMC Plant Biol. 16, 17.  
DePristo, M.A., Banks, E., Poplin, R., Garimella, K.V., Maguire, J.R., Hartl, C., Philippakis, A.A., del Angel, G., Rivas, M.A., Hanna, M., et al. (2011). A framework for variation discovery and genotyping using next-generation DNA sequencing data. Nat. Genet. 43, 491-498.  
Dong, Q., Li, N., Li, X., Yuan, Z., Xie, D., Wang, X., Li, J., Yu, Y., Wang, J., Ding, B., et al. (2018). Genome-wide Hi-C analysis reveals extensive hierarchical chromatin interactions in rice. Plant J. 94, 1141-1156.  
Du, H., and Liang, C. (2019). Assembly of chromosome-scale contigs by efficiently resolving repetitive sequences with long reads. Nat. Commun. 10, 5360.  
Du, H., Yu, Y., Ma, Y., Gao, Q., Cao, Y., Chen, Z., Ma, B., Qi, M., Li, Y., Zhao, X., et al. (2017). Sequencing and de novo assembly of a near complete indica rice genome. Nat. Commun. 8, 15324.  
Duan, P., Xu, J., Zeng, D., Zhang, B., Geng, M., Zhang, G., Huang, K., Huang, L., Xu, R., Ge, S., et al. (2017). Natural Variation in the Promoter of GSE5 Contributes to Grain Size Diversity in Rice. Mol. Plant 10, 685-694.  
Dudchenko, O., Batra, S.S., Omer, A.D., Nyquist, S.K., Hoeger, M., Durand, N.C., Shamim, M.S., Machol, I., Lander, E.S., Aiden, A.P., and Aiden, E.L. (2017). De novo assembly of the Aedes aegypti genome using Hi-C yields chromosome-length scaffolds. Science 356, 92-95.  
Durand, N.C., Robinson, J.T., Shamim, M.S., Machol, I., Mesirov, J.P., Lander, E.S., and Aiden, E.L. (2016). Juicebox Provides a Visualization System for Hi-C Contact Maps with Unlimited Zoom. Cell Syst. 3, 99-101.  
Ellinghaus, D., Kurtz, S., and Willhoeft, U. (2008). LTRharvest, an efficient and flexible software for de novo detection of LTR retrotransposons. BMC Bioinformatics 9, 18.  
Fuentes, R.R., Chebotarov, D., Duitama, J., Smith, S., De la Hoz, J.F., Mohiyyuddin, M., Wing, R.A., McNally, K.L., Tatarinova, T., Grigoriev, A., et al. (2019). Structural variants in 3000 rice genomes. Genome Res. 29, 870-880.  
Garrison, E., Siren, J., Novak, A.M., Hickey, G., Eizenga, J.M., Dawson, E.T., Jones, W., Garg, S., Markello, C., Lin, M.F., et al. (2018). Variation graph toolkit improves read mapping by representing genetic variation in the reference. Nat. Biotechnol. 36, 875-879.  
Goel, M., Sun, H., Jiao, W.B., and Schneeberger, K. (2019). SyRI: finding genomic rearrangements and local sequence differences from whole-genome assemblies. Genome Biol. 20, 277.  
Han, Y., and Wessler, S.R. (2010). MITE-Hunter: a program for discovering miniature inverted-repeat transposable elements from genomic sequences. Nucleic Acids Res. 38, e199.  
He, X., Wang, L., Wu, W., Chen, Z., Lin, F., Cheng, Y., Liu, W., Chen, Y., and Liao, Y. (2014). The progress of mapping, isolation of the genes resisting to blast and their breeding application in rice. Zhongguo Nongxue Tongbao 20, 417-425.

Hickey, G., Heller, D., Monlong, J., Sibbesen, J.A., Sirén, J., Eizenga, J., Dawson, E.T., Garrison, E., Novak, A.M., and Paten, B. (2020). Genotyping structural variants in pangenome graphs using the vg toolkit. Genome Biol. 21, 35.  
Ho, S.S., Urban, A.E., and Mills, R.E. (2020). Structural variation in the sequencing era. Nat. Rev. Genet. 21, 171-189.  
Hu, Z., Wang, W., Wu, Z., Sun, C., Li, M., Lu, J., Fu, B., Shi, J., Xu, J., Ruan, J., et al. (2018). Novel sequences, structural variations and gene presence variations of Asian cultivated rice. Sci. Data 5, 180079.  
Hufnagel, B., Marques, A., Soriano, A., Marquès, L., Divol, F., Doumas, P., Sallet, E., Mancinotti, D., Carrere, S., Marande, W., et al. (2020). High-quality genome sequence of white lupin provides insight into soil exploration and seed quality. Nat. Commun. 11, 492.  
Jayakodi, M., Padmarasu, S., Haberer, G., Bonthala, V.S., Gundlach, H., Monat, C., Lux, T., Kamal, N., Lang, D., Himmelbach, A., et al. (2020). The barley pan-genome reveals the hidden legacy of mutation breeding. Nature 588, 284-289.  
Jeong, H.J., Yang, J., Cho, L.H., and An, G. (2016). OsVIL1 controls flowering time in rice by suppressing OsLF under short days and by inducing Ghd7 under long days. Plant Cell Rep. 35, 905-920.  
Jiao, W.B., and Schneeberger, K. (2020). Chromosome-level assemblies of multiple Arabidopsis genomes reveal hotspots of rearrangements with altered evolutionary dynamics. Nat. Commun. 11, 989.  
Jones, P., Binns, D., Chang, H.-Y., Fraser, M., Li, W., McAnulla, C., McWilliam, H., Maslen, J., Mitchell, A., Nuka, G., et al. (2014). InterProScan 5: genome-scale protein function classification. Bioinformatics 30, 1236-1240.  
Jukes, T.H., and Cantor, C.R. (1969). Evolution of protein molecules. In Mammalian Protein Metabolism, H.N. Munro, ed. (Academic Press), pp. 21-132.  
Kang, H.M., Sul, J.H., Service, S.K., Zaitlen, N.A., Kong, S.Y., Freimer, N.B., Sabatti, C., and Eskin, E. (2010). Variance component model to account for sample structure in genome-wide association studies. Nat. Genet. 42, 348-354.  
Kawahara, Y., de la Bastide, M., Hamilton, J.P., Kanamori, H., McCombie, W.R., Ouyang, S., Schwartz, D.C., Tanaka, T., Wu, J., Zhou, S., et al. (2013). Improvement of the Oryza sativa Nipponbare reference genome using next generation sequence and optical map data. Rice (N. Y.) 6, 4.  
Kent, W.J. (2002). BLAT-the BLAST-like alignment tool. Genome Res. 12, 656-664.  
Kidd, J.M., Graves, T., Newman, T.L., Fulton, R., Hayden, H.S., Malig, M., Kallicki, J., Kaul, R., Wilson, R.K., and Eichler, E.E. (2010). A human genome structural variation sequencing resource reveals insights into mutational mechanisms. Cell 143, 837-847.  
Kim, D., Langmead, B., and Salzberg, S.L. (2015). HISAT: a fast spliced aligner with low memory requirements. Nat. Methods 12, 357-360.  
Kim, D., Paggi, J.M., Park, C., Bennett, C., and Salzberg, S.L. (2019). Graph-based genome alignment and genotyping with HISAT2 and HISAT-genotype. Nat. Biotechnol. 37, 907-915.  
Kobayashi, A., Hori, K., Yamamoto, T., and Yano, M. (2018). Koshihikari: a premium short-grain rice cultivar - its expansion and breeding in Japan. Rice (N. Y.) 11, 15.  
Koren, S., Walenz, B.P., Berlin, K., Miller, J.R., Bergman, N.H., and Phillippy, A.M. (2017). Canu: scalable and accurate long-read assembly via adaptive k-mer weighting and repeat separation. Genome Res. 27, 722-736.  
Kretzschmar, T., Pelayo, M.A., Trijatmiko, K.R., Gabunada, L.F., Alam, R., Jimenez, R., Mendioro, M.S., Slamet-Loedin, I.H., Sreenivasulu, N., Bailey-Serres, J., et al. (2015). A trehalose-6-phosphate phosphatase enhances anaerobic germination tolerance in rice. Nat. Plants 1, 15124.  
Li, H., and Durbin, R. (2009). Fast and accurate short read alignment with Burrows-Wheeler transform. Bioinformatics 25, 1754-1760.  
Li, H., Handsaker, B., Wysoker, A., Fennell, T., Ruan, J., Homer, N., Marth, G., Abecasis, G., and Durbin, R.; 1000 Genome Project Data Processing Subgroup (2009). The sequence alignment/map format and SAMtools. Bioinformatics 25, 2078-2079.

Li, X., Han, H., Chen, M., Yang, W., Liu, L., Li, N., Ding, X., and Chu, Z. (2017). Overexpression of OsDT11, which encodes a novel cysteine-rich peptide, enhances drought tolerance and increases ABA concentration in rice. Plant Mol. Biol. 93, 21-34.  
Liang, C., Mao, L., Ware, D., and Stein, L. (2009). Evidence-based gene predictions in plant genomes. Genome Res. 19, 1912-1923.  
Liu, J., Chen, J., Zheng, X., Wu, F., Lin, Q., Heng, Y., Tian, P., Cheng, Z., Yu, X., Zhou, K., et al. (2017). GW5 acts in the brassinosteroid signalling pathway to regulate grain width and weight in rice. Nat. Plants 3, 17043.  
Liu, Y., Du, H., Li, P., Shen, Y., Peng, H., Liu, S., Zhou, G.A., Zhang, H., Liu, Z., Shi, M., et al. (2020). Pan-Genome of Wild and Cultivated Soybeans. Cell 182, 162-176.e13.  
Lye, Z.N., and Purugganan, M.D. (2019). Copy Number Variation in Domestication. Trends Plant Sci. 24, 352-365.  
Ma, J., and Bennetzen, J.L. (2004). Rapid recent growth and divergence of rice nuclear genomes. Proc. Natl. Acad. Sci. USA 101, 12404-12410.  
Marçais, G., Delcher, A.L., Phillippy, A.M., Coston, R., Salzberg, S.L., and Zimin, A. (2018). MUMmer4: A fast and versatile genome alignment system. PLoS Comput. Biol. 14, e1005944.  
Nonoue, Y., Hori, K., Ono, N., Shibaya, T., Ogiso-Tanaka, E., Mizobuchi, R., Fukuoka, S., and Yano, M. (2019). Detection of heading date QTLs in advanced-backcross populations of an elite indica rice cultivar, IR64. Breed. Sci. 69, 352-358.  
Oikawa, T., Maeda, H., Oguchi, T., Yamaguchi, T., Tanabe, N., Ebana, K., Yano, M., Ebitani, T., and Izawa, T. (2015). The Birth of a Black Rice Gene and Its Local Spread by Introgression. Plant Cell 27, 2401-2414.  
Ou, S., and Jiang, N. (2018). LTR_retriever: A Highly Accurate and Sensitive Program for Identification of Long Terminal Repeat Retrotransposons. Plant Physiol. 176, 1410-1422.  
Ou, S., and Jiang, N. (2019). LTR_FINDER_parallel: parallelization of LTR_FINDER enabling rapid identification of long terminal repeat retrotransposons. Mob. DNA 10, 48.  
Ou, S., Chen, J., and Jiang, N. (2018). Assessing genome assembly quality using the LTR Assembly Index (LAI). Nucleic Acids Res. 46, e126.  
Ou, S., Su, W., Liao, Y., Chougule, K., Agda, J.R.A., Hellinga, A.J., Lugo, C.S.B., Elliott, T.A., Ware, D., Peterson, T., et al. (2019). Benchmarking transposable element annotation methods for creation of a streamlined, comprehensive pipeline. Genome Biol. 20, 275.  
Qu, S., Liu, G., Zhou, B., Bellizzi, M., Zeng, L., Dai, L., Han, B., and Wang, G.L. (2006). The broad-spectrum blast resistance gene Pi9 encodes a nucleotide-binding site-leucine-rich repeat protein and is a member of a multigene family in rice. Genetics 172, 1901-1914.  
Rakocevic, G., Semenyuk, V., Lee, W.P., Spencer, J., Browning, J., Johnson, I.J., Arsenijevic, V., Nadj, J., Ghose, K., Suciu, M.C., et al. (2019). Fast and accurate genomic analyses using genome graphs. Nat. Genet. 51, 354-362.  
Reich, D., Price, A.L., and Patterson, N. (2008). Principal component analysis of genetic data. Nat. Genet. 40, 491-492.  
Sasaki, A., Ashikari, M., Ueguchi-Tanaka, M., Itoh, H., Nishimura, A., Swapan, D., Ishiyama, K., Saito, T., Kobayashi, M., Khush, G.S., et al. (2002). Green revolution: a mutant gibberellin-synthesis gene in rice. Nature 416, 701-702.  
Schatz, M.C., Maron, L.G., Stein, J.C., Hernandez Wences, A., Gurtowski, J., Biggers, E., Lee, H., Kramer, M., Antoniou, E., Ghiban, E., et al. (2014). Whole genome de novo assemblies of three divergent strains of rice, Oryza sativa, document novel gene space of aus and indica. Genome Biol. 15, 506.  
Sedlazeck, F.J., Rescheneder, P., Smolka, M., Fang, H., Nattestad, M., von Haeseler, A., and Schatz, M.C. (2018). Accurate detection of complex structural variations using single-molecule sequencing. Nat. Methods 15, 461-468.  
Shen, R., Wang, L., Liu, X., Wu, J., Jin, W., Zhao, X., Xie, X., Zhu, Q., Tang, H., Li, Q., et al. (2017). Genomic structural variation-mediated allelic suppression causes hybrid male sterility in rice. Nat. Commun. 8, 1310.  
Shi, J., and Liang, C. (2019). Generic Repeat Finder: A High-Sensitivity Tool for Genome-Wide De Novo Repeat Detection. Plant Physiol. 180, 1803-1815.

Simão, F.A., Waterhouse, R.M., Ioannidis, P., Kriventseva, E.V., and Zdobnov, E.M. (2015). BUSCO: assessing genome assembly and annotation completeness with single-copy orthologs. Bioinformatics 31, 3210-3212.  
Smit, A., Hubley, R., and Green, P. (2013-2015). RepeatMasker Open-4.0. https://www.repeatmasker.org.  
Song, J.M., Guan, Z., Hu, J., Guo, C., Yang, Z., Wang, S., Liu, D., Wang, B., Lu, S., Zhou, R., et al. (2020). Eight high-quality genomes reveal pan-genome architecture and ecotype differentiation of Brassica napus. Nat. Plants 6, 34-45.  
Stanke, M., and Morgenstern, B. (2005). AUGUSTUS: a web server for gene prediction in eukaryotes that allows user-defined constraints. Nucleic Acids Res. 33, W465-7.  
Stein, J.C., Yu, Y., Copetti, D., Zwickl, D.J., Zhang, L., Zhang, C., Chougule, K., Gao, D., Iwata, A., Goicoechea, J.L., et al. (2018). Genomes of 13 domesticated and wild rice relatives highlight genetic conservation, turnover and innovation across the genus Oryza. Nat. Genet. 50, 285-296.  
Su, W., Gu, X., and Peterson, T. (2019). TIR-Learner, a New Ensemble Method for TIR Transposable Element Annotation, Provides Evidence for Abundant New Transposable Elements in the Maize Genome. Mol. Plant 12, 447-460.  
Sun, S., Zhou, Y., Chen, J., Shi, J., Zhao, H., Zhao, H., Song, W., Zhang, M., Cui, Y., Dong, X., et al. (2018). Extensive intraspecific gene order and gene structural variations between Mo17 and other maize genomes. Nat. Genet. 50, 1289-1295.  
Thorvaldsdóttir, H., Robinson, J.T., and Mesirov, J.P. (2013). Integrative Genomics Viewer (IGV): high-performance genomics data visualization and exploration. Brief. Bioinform. 14, 178-192.  
Trapnell, C., Williams, B.A., Pertea, G., Mortazavi, A., Kwan, G., van Baren, M.J., Salzberg, S.L., Wold, B.J., and Pachter, L. (2010). Transcript assembly and quantification by RNA-Seq reveals unannotated transcripts and isoform switching during cell differentiation. Nat. Biotechnol. 28, 511-515.  
Walkowiak, S., Gao, L., Monat, C., Haberer, G., Kassa, M.T., Brinton, J., Ramirez-Gonzalez, R.H., Kolodziej, M.C., Delorean, E., Thambugala, D., et al. (2020). Multiple wheat genomes reveal global variation in modern breeding. Nature 588, 277-283.  
Wang, Y., Tang, H., Debarry, J.D., Tan, X., Li, J., Wang, X., Lee, T.H., Jin, H., Marler, B., Guo, H., et al. (2012). MCScanX: a toolkit for detection and evolutionary analysis of gene synteny and collinearity. Nucleic Acids Res. 40, e49.  
Wang, Y., Xiong, G., Hu, J., Jiang, L., Yu, H., Xu, J., Fang, Y., Zeng, L., Xu, E., Xu, J., et al. (2015). Copy number variation at the GL7 locus contributes to grain size diversity in rice. Nat. Genet. 47, 944-948.  
Wang, J., Tao, F., Marowsky, N.C., and Fan, C. (2016). Evolutionary Fates and Dynamic Functionalization of Young Duplicate Genes in Arabidopsis Genomes. Plant Physiol. 172, 427-440.  
Wang, W., Mauleon, R., Hu, Z., Chebotarov, D., Tai, S., Wu, Z., Li, M., Zheng, T., Fuentes, R.R., Zhang, F., et al. (2018). Genomic variation in 3,010 diverse accessions of Asian cultivated rice. Nature 557, 43-49.  
Wang, M., Tu, L., Yuan, D., Zhu, D., Shen, C., Li, J., Liu, F., Pei, L., Wang, P., Zhao, G., et al. (2019). Reference genome sequences of two cultivated allotetraploid cottons, Gossypium hirsutum and Gossypium barbadense. Nat. Genet. 51, 224-229.  
Wang, H., Zhang, Y., Xiao, N., Zhang, G., Wang, F., Chen, X., and Fang, R. (2020). Rice GERMIN-LIKE PROTEIN 2-1 Functions in Seed Dormancy under the Control of Abscisic Acid and Gibberellic Acid Signaling Pathways. Plant Physiol. 183, 1157-1170.  
Weischenfeldt, J., Simmons, O., Spitz, F., and Korbel, J.O. (2013). Phenotypic impact of genomic structural variation: insights from and for human disease. Nat. Rev. Genet. 14, 125-138.  
Wing, R.A., Purugganan, M.D., and Zhang, Q. (2018). The rice genome revolution: from an ancient grain to Green Super Rice. Nat. Rev. Genet. 19, 505-517.  
Xia, L., Zou, D., Sang, J., Xu, X., Yin, H., Li, M., Wu, S., Hu, S., Hao, L., and Zhang, Z. (2017). Rice Expression Database (RED): An integrated RNA-Seq-derived gene expression database for rice. J. Genet. Genomics 44, 235-241.  
Xie, X., Yoneyama, K., and Yoneyama, K. (2010). The strigolactone story. Annu. Rev. Phytopathol. 48, 93-117.

Xie, Y., Wu, G., Tang, J., Luo, R., Patterson, J., Liu, S., Huang, W., He, G., Gu, S., Li, S., et al. (2014). SOAPdenovo-Trans: de novo transcriptome assembly with short RNA-Seq reads. Bioinformatics 30, 1660-1666.  
Xiong, W., He, L., Lai, J., Dooner, H.K., and Du, C. (2014). HelitronScanner uncovers a large overlooked cache of Helitron transposons in many plant genomes. Proc. Natl. Acad. Sci. USA 111, 10263-10268.  
Yang, L., Luquette, L.J., Gehlenborg, N., Xi, R., Haseley, P.S., Hsieh, C.H., Zhang, C., Ren, X., Protopopov, A., Chin, L., et al. (2013). Diverse mechanisms of somatic structural variations in human cancer genomes. Cell 153, 919-929.  
Yang, N., Liu, J., Gao, Q., Gui, S., Chen, L., Yang, L., Huang, J., Deng, T., Luo, J., He, L., et al. (2019a). Genome assembly of a tropical maize inbred line provides insights into structural variation and crop improvement. Nat. Genet. 51, 1052-1059.  
Yang, Z., Ge, X., Yang, Z., Qin, W., Sun, G., Wang, Z., Li, Z., Liu, J., Wu, J., Wang, Y., et al. (2019b). Extensive intraspecific gene order and gene structural variations in upland cotton cultivars. Nat. Commun. 10, 2989.  
Yao, W., Li, G., Yu, Y., and Ouyang, Y. (2018). funRiceGenes dataset for comprehensive understanding and application of rice functional genes. Gigascience 7, 1-9.  
Yin, X., Liu, X., Xu, B., Lu, P., Dong, T., Yang, D., Ye, T., Feng, Y.Q., and Wu, Y. (2019). OsMADS18, a membrane-bound MADS-box transcription factor, modulates plant architecture and the abscisic acid response in rice. J. Exp. Bot. 70, 3895-3909.

Yu, P., Wang, C.H., Xu, Q., Feng, Y., Yuan, X.P., Yu, H.Y., Wang, Y.P., Tang, S.X., and Wei, X.H. (2013). Genome-wide copy number variations in Oryza sativa L. BMC Genomics 14, 649.  
Yuan, S., Wang, Y., Zhang, C., He, H., and Yu, S. (2020). Genetic Dissection of Seed Dormancy using Chromosome Segment Substitution Lines in Rice (Oryza sativa L.). Int. J. Mol. Sci. 21, 1344.  
Zhang, J., Chen, L.L., Xing, F., Kudrna, D.A., Yao, W., Copetti, D., Mu, T., Li, W., Song, J.M., Xie, W., et al. (2016). Extensive sequence divergence between the reference genomes of two elite indica rice varieties Zhenshan 97 and Minghui 63. Proc. Natl. Acad. Sci. USA 113, E5163-E5171.  
Zhang, Q., Liang, Z., Cui, X., Ji, C., Li, Y., Zhang, P., Liu, J., Riaz, A., Yao, P., Liu, M., et al. (2018). N $^6$ -Methyladenine DNA Methylation in Japonica and Indica Rice Genomes and Its Association with Gene Expression, Plant Development, and Stress Responses. Mol. Plant 11, 1492-1508.  
Zhao, Q., Feng, Q., Lu, H., Li, Y., Wang, A., Tian, Q., Zhan, Q., Lu, Y., Zhang, L., Huang, T., et al. (2018). Pan-genome analysis highlights the extent of genomic variation in cultivated and wild rice. Nat. Genet. 50, 278-284.  
Zhou, Y., Minio, A., Massonnet, M., Solares, E., Lv, Y., Beridze, T., Cantu, D., and Gaut, B.S. (2019). The population genetics of structural variants in grapevine domestication. Nat. Plants 5, 965-979.  
Zhou, Y., Chebotarov, D., Kudrna, D., Llaca, V., Lee, S., Rajasekar, S., Mohammed, N., Al-Bader, N., Sobel-Sorenson, C., Parakkal, P., et al. (2020). A platinum standard pan-genome resource that represents the population structure of Asian rice. Sci. Data 7, 113.

# STAR\*METHODS

# KEY RESOURCES TABLE

<table><tr><td>REAGENT or RESOURCE</td><td>SOURCE</td><td>IDENTIFIER</td></tr><tr><td colspan="3">Deposited data</td></tr><tr><td>Rice: PacBio, BioNano, Hi-C and DNA sequencing data</td><td>This paper</td><td>BioProject: PRJCA002103</td></tr><tr><td>Rice: RNA sequencing data</td><td>This paper</td><td>BioProject: PRJCA002103</td></tr><tr><td>Rice: Genome assemblies</td><td>This paper</td><td>http://www.ricerc.com</td></tr><tr><td>Rice: Genome and TE annotations</td><td>This paper</td><td>http://www.ricerc.com</td></tr><tr><td>SV catalog</td><td>This paper</td><td>http://www.ricerc.com</td></tr><tr><td>Gene CNV catalog</td><td>This paper</td><td>http://www.ricerc.com</td></tr><tr><td>dSV catalog</td><td>This paper</td><td>http://www.ricerc.com</td></tr><tr><td>dSVs frequency among Oryza.sativa subpopulations and wild rice population</td><td>This paper</td><td>Table S5</td></tr><tr><td>SV hotspot regions</td><td>This paper</td><td>Table S3</td></tr><tr><td>SNP dataset</td><td>This paper</td><td>http://www.ricerc.com</td></tr><tr><td>Indel dataset</td><td>This paper</td><td>http://www.ricerc.com</td></tr><tr><td>Graph-based genome</td><td>This paper</td><td>http://www.ricerc.com</td></tr><tr><td colspan="3">Oligonucleotides</td></tr><tr><td>Expression verification for Os06 g13470</td><td>This paper</td><td>N/A</td></tr><tr><td>Forward:AGAGTTTCCCTGACAAGAGTG</td><td></td><td></td></tr><tr><td>Expression verification for Os06 g13470</td><td>This paper</td><td>N/A</td></tr><tr><td>Reverse:ACTAAGCACCATCTGACCACC</td><td></td><td></td></tr><tr><td>Expression verification for OsVIL1</td><td>This paper</td><td>N/A</td></tr><tr><td>Forward:ATGACTCACCTCGGCAAAC</td><td></td><td></td></tr><tr><td>Expression verification for OsVIL1</td><td>This paper</td><td>N/A</td></tr><tr><td>Reverse: ACTGGCTTCGTCGTTGTCA</td><td></td><td></td></tr><tr><td>DNA copy number variation for OsVIL1</td><td>This paper</td><td>N/A</td></tr><tr><td>Forward:ATGCCACCTAAAGTGTGCTCT</td><td></td><td></td></tr><tr><td>DNA copy number variation for OsVIL1</td><td>This paper</td><td>N/A</td></tr><tr><td>Reverse:CAGTGACAAACGCTCACACA</td><td></td><td></td></tr><tr><td>Expression verification for OsMADS18</td><td>This paper</td><td>N/A</td></tr><tr><td>Forward:TGCACATACGGTTCATGGCT</td><td></td><td></td></tr><tr><td>Expression verification for OsMADS18</td><td>This paper</td><td>N/A</td></tr><tr><td>Reverse:GGGGACACAAGCAACCTACA</td><td></td><td></td></tr><tr><td>DNA copy number variation for OsMADS18</td><td>This paper</td><td>N/A</td></tr><tr><td>Forward: CCCATTTCCATCTTCCCCGA</td><td></td><td></td></tr><tr><td>DNA copy number variation for OsMADS18</td><td>This paper</td><td>N/A</td></tr><tr><td>Reverse:ATCTTGTTCTCGATCCGCCG</td><td></td><td></td></tr><tr><td>Expression verification for Kala4</td><td>This paper</td><td>N/A</td></tr><tr><td>Forward:CTGCATGACCTACGCCTTTC</td><td></td><td></td></tr><tr><td>Expression verification for Kala4</td><td>This paper</td><td>N/A</td></tr><tr><td>Reverse:ATCAGTGGTTCCCAGCTCAA</td><td></td><td></td></tr><tr><td>DNA copy number variation for Kala4</td><td>This paper</td><td>N/A</td></tr><tr><td>Forward:GTACCAGCAGTTCACCACGA</td><td></td><td></td></tr><tr><td>DNA copy number variation for Kala4</td><td>This paper</td><td>N/A</td></tr><tr><td>Reverse:GGACTTGACAGAACCGCTGA</td><td></td><td></td></tr><tr><td colspan="3">Software and Algorithms</td></tr><tr><td>Hisat2</td><td>Kim et al., 2015</td><td>https://github.com/DaehwanKimLab/hisat2</td></tr><tr><td>Cufflinks</td><td>Trapnell et al., 2010</td><td>https://github.com/cole-trapnell-lab/cufflinks</td></tr></table>

(Continued on next page)

Continued  

<table><tr><td>REAGENT or RESOURCE</td><td>SOURCE</td><td>IDENTIFIER</td></tr><tr><td>CANU v1.7.1</td><td>Koren et al., 2017</td><td>https://github.com/marbl/canu/</td></tr><tr><td>HERA</td><td>Du and Liang, 2019</td><td>https://github.com/liangclab/HERA/</td></tr><tr><td>MUMmer4</td><td>Marçais et al., 2018</td><td>https://github.com/mummer4/mummer</td></tr><tr><td>BWA</td><td>Li and Durbin, 2009</td><td>https://sourceforge.net/projects/bio-bwa/</td></tr><tr><td>SAMtools</td><td>Li et al., 2009</td><td>https://sourceforge.net/projects/samtools/</td></tr><tr><td>GATK 2.7.2</td><td>DePristo et al., 2011</td><td>N/A</td></tr><tr><td>ADMIXTURE</td><td>Alexander et al., 2009</td><td>http://dalexander.github.io/admixture/</td></tr><tr><td>Augustus</td><td>Stanke and Morgenstern, 2005</td><td>https://sourceforge.net/projects/augustus/</td></tr><tr><td>SOAPdenovo-trans</td><td>Xie et al., 2014</td><td>https://github.com/aquaskyline/SOAPdenovo-Trans</td></tr><tr><td>Interproscan v5.0</td><td>Jones et al., 2014</td><td>https://www.msi.umn.edu/sw/interproscan</td></tr><tr><td>BUSCO</td><td>Simão et al., 2015</td><td>https://busco.ezlab.org/</td></tr><tr><td>EDTA v1.3</td><td>Ou et al., 2019</td><td>https://github.com/oushujun/EDTA/releases</td></tr><tr><td>LTRharvest v1.5.10</td><td>Ellinghaus et al., 2008</td><td>https://www.zbh.uni-hamburg.de/en/forschung/gi/software/ltrharvest.html</td></tr><tr><td>LTR_FINDER_parallel v1.0</td><td>Ou and Jiang, 2019</td><td>https://github.com/oushujun/LTR_FINDER_parallel</td></tr><tr><td>LTR_retriever v2.6</td><td>Ou and Jiang, 2018</td><td>https://github.com/oushujun/LTR_retriever</td></tr><tr><td>Generic Repeat Finder v1.0</td><td>Shi and Liang, 2019</td><td>https://github.com/bioinfolabmu/GenericRepeatFinder</td></tr><tr><td>TIR-Learner v1.23</td><td>Su et al., 2019</td><td>N/A</td></tr><tr><td>MITE-Hunter v1.0</td><td>Han and Wessler, 2010</td><td>http://target.iplantcollaborative.org/mite_hunter.html</td></tr><tr><td>HelitronScanner v1.0</td><td>Xiong et al., 2014</td><td>https://sourceforge.net/projects/helitronscanner/files/</td></tr><tr><td>RepeatMasker v4.0.9</td><td>Smit et al., 2013-2015</td><td>http://repeatmasker.org/</td></tr><tr><td>MCscan python version</td><td>Wang et al., 2012</td><td>https://github.com/tanghaibao/jcvi/wiki/MCscan-(Python-version)</td></tr><tr><td>SyRI</td><td>Goel et al., 2019</td><td>https://schneebergerlab.github.io/syri/fileformat.html.</td></tr><tr><td>NGMLR</td><td>Sedlazeck et al., 2018</td><td>https://github.com/philres/ngmlr</td></tr><tr><td>Integrative Genomics Viewer</td><td>Thorvaldsdóttir et al., 2013</td><td>http://software.broadinstitute.org/software/igv/</td></tr><tr><td>Juicer</td><td>Durand et al., 2016</td><td>https://github.com/aidenlab/juicer</td></tr><tr><td>3D-DNA</td><td>Dudchenko et al., 2017</td><td>https://github.com/aidenlab/3d-dna</td></tr><tr><td>Sniffle</td><td>Sedlazeck et al., 2018</td><td>https://github.com/fritzsedlazeck/Sniffles</td></tr><tr><td>Blat</td><td>Kent, 2002</td><td>http://genome.ucsc.edu/FAQ/FAQblat.html</td></tr><tr><td>Variation graph toolkit</td><td>Garrison et al., 2018</td><td>https://github.com/vgteam/vg</td></tr><tr><td>EMMAX v20120210</td><td>Kang et al., 2010</td><td>http://csg.sph.umich.edu/kang/emmax/download/index.html</td></tr><tr><td>EIGENSOFT v5.0.2</td><td>Reich et al., 2008</td><td>https://reich.hms.harvard.edu/software</td></tr></table>

# RESOURCEAVAILABILITY

# Lead contact

Further information and requests for reagents may be directed to, and will be fulfilled by the Lead Contact, Shigui Li (lishigui@sicau.edu.cn).

# Materials availability

This study did not generate new unique reagents.

# Data and code availability

All sequencing data generated in this paper have been deposited into the National Genomics Data Center (https://bigd/big.ac.cn/?lang=en) and are accessible through the BioProject number: PRJCA002103. All genome assemblies/annotations, SVs, gene CNVs, SNPs, and the graph-based genome are available at the Rice Resource Center (https://www.ricerca.com).

# EXPERIMENTAL MODEL AND SUBJECT DETAILS

The 33 accessions of rice were sown on April 11th, 2018, at Wenjiang, Chengdu, China (103°51'E, 30°43'N). All accessions used in this study are listed in Table S1.

For the long-read and short-read sequencing of DNA, samples were collected from the accessions in this study. Library construction and sequencing were performed by the BGI company (BGI, Shenzhen, China). For Hi-C sequencing, fresh leaves were collected from three-week-old seedlings of TM and CG14; the libraries for Hi-C sequencing were constructed using the Mbol restriction endonuclease, and paired-end sequencing  $(2 \times 250$  bp) was conducted on the NovaSeq 6000 platform. For RNA sequencing, RNA extraction of plant materials was carried out using TRIzol (Invitrogen) from 21-day-old plants. The tissues collected for RNA sequencing included shoots and root for 33 accessions, and 29 samples from R527 (including leaf, panicle, stem, and caryopsis at different stages, as well as shoots and roots treated with different abiotic stress conditions) seeing in Table S4. RNA-seq libraries were prepared with an insert size of 300 bp and sequenced on BGIseq500 platform (BGI, Shenzhen, China). For BioNano, fresh leaf tissues from 10-day-old seedlings of three accessions (9311, 02428, and DG) were collected to extract high-molecular-weight DNA; DNA labeling (with DLE-1 nicking endonuclease) was performed according to the standard protocols provided by BioNano Genomics. Labeled DNA samples were loaded and analyzed on the SAPHYR system (BioNano Genomics). All single molecules whose length exceeded  $100\mathrm{kb}$  were used for further analysis. For experimental analysis of DNA copy number variation and expression level, DNA and RNA was respectively extracted using DNeasy Plant Mini Kit (Qigen), and TRIzol (Invitrogen) from the plant materials seeing in Table S4.

# METHOD DETAILS

# Investigation of agronomic traits

Seeds of the 33 accessions were sown on April  $11^{\text{th}}$ , 2018, at Wenjiang, Chengdu, China (103°51'E, 30°43'N). The agronomic traits including heading date, plant height, tiller number, panicle length, grain number per panicle, grain length, grain width, and 1,000-grain weight (Table S1) were examined at the mature stage.

# Preparation of short-read sequencing libraries

High-molecular-weight genomic DNA was extracted from 10-day-old leaves of the 30 accessions following a standard CTAB (hexadecyltrimethylammonium bromide) protocol. The sequencing libraries with a medium insert of 300 bp were prepared using NEBNext Ultra DNA Library Prep Kits for Illumina sequencing. Sequencing was performed on the BGIseq500 platform (BGI, Shenzhen, China). The short-reads were filtered by removing adaptor contamination and low-quality reads with base N's or more than  $10\%$  of bases with a quality score  $< 20$ .

# RNA sequencing and data analysis

RNA extraction of plant materials was carried out using TRIzol (Invitrogen) from 21-day-old plants. The tissues collected for RNA sequencing included shoots and roots from 33 accessions, and 29 samples prepared from diverse rice tissues from the R527 accession (including leaf, panicle, and caryopsis at different stages, as well as shoots and roots treated with different abiotic stresses, also seeing in Table S4). RNA-seq libraries were prepared with an insert size of 300 bp and sequenced on BGIseq500 platform (BGI, Shenzhen, China). RNA-seq data were processed using the Hisat2 (Kim et al., 2015) and Cufflinks pipelines (Trapnell et al., 2010). The RNA-seq reads were mapped to the Nipponbare genome (IRGSP1.0) (Kawahara et al., 2013) for correlation analysis between the presence of a dSV and its corresponding gene expression levels, and for the correlation analysis between the gene copy number and its expression levels. The RNA-seq reads of 29 samples from R527 were mapped to R527 assembly. FPKM (fragments per kilobase of exon per million fragments mapped) values for each transcript were calculated using Cufflinks (Trapnell et al., 2010).

# Long-reads sequencing and de novo genome assembly

The 30-Kbp SMRTbell sequencing libraries were prepared using the standard protocol from PacBio and sequenced on the PacBio RS II system with P5 Polymerase Binding and C3 Chemistry Kits as well as P6 Polymerase Binding and C4 Chemistry Kits. The raw PacBio reads were error-corrected and assembled using CANU (v1.7.1) to get the raw contigs (Koren et al., 2017) with parameters set as: useGrid = true; minThreads = 4; genomeSize = 400 m; minOverlapLength = 700; minReadLength = 1000, other parameters were default. The corrected long-reads and assembled contigs by CANU were further assembled into super contigs using HERA (Du and Liang, 2019). All super contigs from GJ accessions were respectively aligned to Nipponbare genome (IRGSP1.0) using Mummer (v4.0) (Marçais et al., 2018) to construct pseudo-chromosomes, and all super contigs from other accessions were aligned to R498 genome (Du et al., 2017) for constructing pseudo-chromosomes. The parameters used in Mummer (Marçais et al., 2018) were set as: -mum -mincluster = 1000 and the HERA were set as: InterIncluded_Side = 30000; InterIncluded_Identity = 99; InterIncluded_Coverage = 99; MinIdentity = 97; MinCoverage = 90; MinLength = 5000; MinIdentity_Overlap = 97; MinOverlap_Overlap = 1000; MaxOverhang_Overlap = 100; MinExtend_Overlap = 500.

# Short-reads data processing

Short-reads resequencing data were aligned to reference or the de novo assemblies using BWA (Li and Durbin, 2009) with the MEM algorithm. Then the mapping results were filtered and sorted using SAMtools (Li et al., 2009), retaining reads with a mapping quality over 30. We used the SAMtools rmdup function to remove potential PCR duplicates and erroneous mismatches around small-scale insertions and deletions were removed using the IndelRealigner tool in GATK (v2.7.2) (DePristo et al., 2011) with default parameters. Nucleotide variants were detected using the UnifiedGenotyper tool in GATK with the parameters: "-stand_call_conf 50.0 -stand_ emit_conf 10.0 -dcov 1000 -A Coverage -A AlleleBalance." Then the obtained variants were classified and tagged using VariantFiltration tools in GATK.

# Construction of BioNano optical maps

Fresh leaf tissues from 10-day-old seedlings of three accessions including 9311, 02428 and DG were collected, and high-molecular-weight DNA extraction and DNA labeling (with DLE-1 nicking endonuclease) were both performed according to the standard protocols provided by BioNano Genomics. Labeled DNA samples were loaded and run on the SAPHYR system (BioNano Genomics). All single molecules whose length exceeded  $100\mathrm{kb}$  were collected and assembled by RefAligner (https://bionanogenomics.com/) and Assembler from BioNano Solve3.1_08232017 software. The assembly parameters were set as: -U -d -T 20 -j 4 -N 10 -i 5. The assembled BioNano restriction maps were aligned to the assemblies of 9311, 02428, and DG to check the assembly correctness and to detect InDels using RefAligner to assess the quality of assemblies.

# Population structure analysis

The SNPs in 32 O. sativa accessions along with 3010 samples from the 3K-RG dataset (Wang et al., 2018) were genotyped using GATK UnifiedGenotyper, as described by Chen et al. (2020), and generated a dataset with 342,462 SNP markers. We performed population structure inference using ADMIXTURE (Alexander et al., 2009). When assigning 9 ancestries  $(\mathrm{K} = 9)$ , all 9 subpopulations defined by Wang et al. (2018) emerged. The subpopulation origins of the 32 accessions were confirmed (for accessions already included in the 3K-RG accessions) or defined according to their ancestral score provided by ADMIXTURE.

# Gene annotations

Protein-coding genes were annotated using the ab initio gene predictions software Augustus (Stanke and Morgenstern, 2005) and evidence-based pipeline Gramene (Liang et al., 2009), with rice and monocot cDNAs/ESTs downloaded from GenBank (https://www.ncbi.nlm.nih.gov/); protein sequences were downloaded from SwissProt (https://www.uniprot.org). A total of 617 rice RNA-seq datasets were downloaded from the GenBank SRA (short-read archive) database (Table S2), and transcript contigs were assembled using SOAPdenovo-trans (Xie et al., 2014). The assembled transcript contigs  $>200$  bp, and annotated transcripts of Nipponbare (V.7.0, http://rice.plantbiology.msu.edu) were used as evidence for gene annotation. The protein domain information was annotated using Interproscan 5.0 (Jones et al., 2014). The protein-coding annotations were evaluated using Benchmarking universal single-copy orthologs (BUSCO) (Simão et al., 2015).

# Repeat sequence annotation

Transposable elements of the 33 rice assemblies were annotated using EDTA (v1.3) (Ou et al., 2019), which combined the raw predictions of LTRharvest (v1.5.10) (Ellinghaus et al., 2008), LTR_FINDER_parallel (v1.0) (Ou and Jiang, 2019), LTR_retriever (v2.6) (Ou and Jiang, 2018), Generic Repeat Finder (v1.0) (Shi and Liang, 2019), TIR-Learner (v1.23) (Su et al., 2019), MITE-Hunter (v1.0) (Han and Wessler, 2010), and HelitronScanner (v1.0) (Xiong et al., 2014) with extra basic and advanced filters. The EDTA-generated nonredundant TE library of each genome were masked using the manually curated rice TE library (rice6.9.5.liban) included in the EDTA package (https://github.com/oushujun/EDTA). The unmasked sequences were considered previously unidentified TE sequences and combined from the 33 TE libraries. Then redundant previously unidentified TEs were removed using the cleanup_nested.pl script in the EDTA package with parameters "-cov 0.9 -minlen 80 -iter 8." Finally, non-redundant previously unidentified TEs were combined with the curated TE library (rice6.9.5.liban) and a pan-genome TE library was formed. The pan-genome TE library was then used to annotate whole-genome TEs in the 33 rice assemblies using RepeatMasker (v4.0.9) (Smit et al., 2013-2015) with parameters "-q -no_is -norna -nolow -div 40 -cutoff 225."

# Estimation of TE duplication times

Sequences of tandem genes were first extracted from the Nipponbare genome (IRGSP1.0) using the call_seq_by_list.pl script in the LTR_retriever package. Extracted nucleotide sequences were used as queries to blast against the other 32 rice assemblies. Full-length matches were determined when  $80\%$  of the query matched the subject sequences. The blast hit identity of each full-length match was used to estimate its divergence (K) to the query sequence based on the Jukes-Cantor model (Jukes and Cantor, 1969), with the equation  $\mathrm{K} = -3 / 4^{*}\log (1 - 4^{*}(1 - \text{identity}\%) / 3)$ . Then the ages of each duplicated gene (T) were estimated using  $\mathrm{T} = \mathrm{K} / 2\mu$ , where  $\mu$  is the nucleotide substitution rate in rice and estimated as  $1.3 \times 10^{-8}$  per bp per year (Ma and Bennetzen, 2004). Insertion time of LTR retrotransposons were estimated by LTR_retriever using the same mutation rate, and divergence was estimated between the left and right LTR sequence of each intact element.

# Gene-based pan-genome construction

We employed a stepwise strategy to build the gene-based pan-genome. First, we carried out pairwise collinearity analysis for the 33 assemblies using MCscan (python version) (Wang et al., 2012) with default parameters. We used Nipponbare genes (V.7.0 http://rice.plantbiology.msu.edu) (without genes encoding transposons or retrotransposons) as the base, and these genes from 32 assemblies were added in a stepwise manner: a gene will be added into gene list and assigned a new locus ID if it has no collinear gene with any genes in the gene list produced by the preceding step. This operation was repeated until all genes from 32 assemblies had been added to the pan-genome.

# SV identification

All 32 assemblies were aligned to the Nipponbare genome (IRGSP1.0) using Mummer (v 4.0) with the parameters: -l 50 -c 100 -max-match. The raw alignments results were further filtered using delta-filtre with parameters: -m -i 90 -l 100. The resulting filtered delta files were used to detect structural variations using the SyRI pipeline with default parameters (Goel et al., 2019). The detected variations from SyRI comprise a two hierarchy structure: genome rearrangements and sequential variations (which can occur in both rearrangement regions and syntenic regions). The rearrangements and sequential variations in syntenic regions were used for the SV convert, the sequential variants which are embedded in the rearrangements were not included for further analysis.

According to the definitions of sequence variation in SyRI outputs, we converted these variations into three types of SVs: PAVs (Presence/Absence Variations), inversions, and translocations. The CPL, DEL, DUP/INVDP (loss) variants, and the Nipponbare sequences in HDR, NOTAL, and TDM were converted as Absence SVs (relative to Nipponbare) in a given accession. The CPG, INS, DUP/INVDP (gain) variants, and the query sequences in HDR, NOTAL, and TDM were converted as Presence SVs (relative to Nipponbare) in a given accession. The INV variants were regarded as inversion SVs relative to Nipponbare; the TRANS and INVTR were both regarded as translocation SVs relative to Nipponbare in a given accession. The identical type SVs with continuous (or overlapped) coordinates on a reference or query assembly were merged as a single SV which covered all sequence of continuous SVs. For details about these definitions, refer to: https://schneebergerlab.github.io/syri/fileformat.html.

# SV validation

A total of 60 SVs including insertions and inversions were randomly selected from SVs between the Nipponbare and TM or between the Nipponbare and CG14 assemblies, including 30 SVs with length ranging from 2-8 Kbp, and SVs with length ranging from 238 Kbp to 5.2 Mbp. For the SVs less than 8 Kbp, the raw long-reads from TM and CG14 were aligned to the Nipponbare genome (IRGSP 1.0) using NGMLR (Sedlazeck et al., 2018) to check the Absence SV (relative to Nipponbare) in the CG14 and TM assemblies. The raw long-reads from Nipponbare (Zhang et al., 2018) were aligned to the CG14 and TM assemblies to check the Presence SV (relative to Nipponbare) in the CG14 and TM assemblies. The alignments were manually inspected using the Integrative Genomics Viewer (Thorvaldsdóttir et al., 2013).

For validation of SVs  $>200$  Kbp—owing to the length limitation of the raw reads—we used a chromatin interaction heatmap at 5 Kbp resolution based on Hi-C sequencing data. Briefly, we collected fresh leaves of three-week-old seedlings of TM and CG14 for the Hi-C sequencing library construction; the libraries for Hi-C sequencing were constructed using the Mbol restriction endonuclease, and paired-end sequencing  $(2\times 250\mathrm{bp})$  was conducted on the NovaSeq 6000 platform. The Hi-C reads from TM and CG14 assemblies were aligned to the Nipponbare genome to check the Absence SV (relative to Nipponbare) and inversion SV and in the CG14 and TM assemblies. The Hi-C reads from the Nipponbare genome (Dong et al., 2018) were aligned to the TM and CG14 assemblies to check the Presence SVs (relative to Nipponbare) in the CG14 and TM assemblies, using Juicer (Durand et al., 2016). The alignments were filtered using 3D-DNA (Dudchenko et al., 2017), and the reads with a MAPQ quality score less than 30 were discarded. The large SVs were then manually checked using the Juicerbox heatmap (Durand et al., 2016).

# SV comparisons

Using the Nipponbare genome as the reference, we called SVs using long-reads from 32 accessions using the NGMLR/Sniffle pipeline (Sedlazeck et al., 2018), and downloaded SVs previously identified based on short-reads from the 3K-RG panel dataset (Fuentes et al., 2019). We next compared PAVs from these two SVs callsets with the PAVs obtained based on the SyRI pipeline and high-quality assemblies of O. sativa accession. For the Absence SVs relative to Nipponbare, if the overlapping ratio of two Absence SVs (the length of the overlapping sequence / the length of non-redundant genome segment covered by the two SVs) exceeded  $90\%$ , then we determined that these two Absence SVs from two callsets were the same Absence SV. For Presence SVs relative to Nipponbare, if the overlapping ratio of two Presence SVs (the length of shorter SV / the length of longer SV) exceeded  $90\%$ , and their positions on Nipponbare genome was less than 5bp, then we determined that two Presence SVs from two callsets were the same Presence SV.

# Identification of SV hotspot regions

We calculated the distribution of SV breakpoints for each 200 Kbp window (with a 100 Kbp step size) along each chromosome. Then, all 200 Kbp windows were ranked in descending order according to the numbers of SVs within the window. We defined the top  $10\%$  of all windows with the highest frequency of SV breakpoints as SV hotspots, then merged all of the continuous hotspot windows as the "hotspot regions."

# Merging SV and inferring the derived SVs

For merging SVs (including Absence, Inversion and Translocation SVs) relative to Nipponbare from the 32 accessions, the following criterion was used: two SVs were merged as one SV if the overlapping ratio of these two SVs (the length of the overlapping sequence/ the length of non-redundant genome segment covered by the two SVs) exceeded  $90\%$ . For merging Presence SVs from the 32 accessions, the following criterion was used: if their overlapping ratio (the length of the shorter SV/the length of longer SV) exceeded  $90\%$ , and their positions on the Nipponbare genome were less than 5bp, two Presence SVs were merged as one Presence SV.

The O. glaberrima accession CG14 was used as an outgroup to infer the ancestral and derived state of SNPs and SVs. For inference of SV representing the derived state (dSV): if one SV exists in varied states among the O. sativa accessions, then the same state as in O. glaberrima (CG14) was defined as the ancestral state. To infer the derived allele for SNPs, we only considered the bi-allelic SNPs among the 32 O. sativa accessions. Potential impacts of the SNPs on non-TE coding genes (V7.0) were annotated using snpEff (Version 3.3) (36) with default parameters, based on the gene annotation for the Nipponbare genome (V7.0).

# Distribution of SVs relative to gene position

Based on the genomic region overlapping with dSVs, we classified SVs into five categories: SVs sharing overlap with  $\pm 2$  Kbp of coding regions (2 Kbp upstream of the start codon, and 2 Kbp downstream of the stop codon), coding region, intron (both self-explanatory), and intergenic region (outside genic regions (including coding region, intron and  $\pm 2$  Kbp of coding regions)). If an SV shared overlap with two or more different genomic regions, this SV was simultaneously classified among the SVs sharing overlap with the different genomic regions (that is, if an SV sharing overlap with coding region and 2 Kbp upstream, this SV was simultaneously classified among SVs overlapping with the coding region and also among the SVs overlapped with the 2 Kbp upstream sequence). We then calculated the percentage of each SV category among all SVs.

# Identification of gene CNVs

We analyzed gene copy number variations by aligning the predicted protein sequences to the genome assemblies to eliminate undue influence from annotation uncertainty and/or sequence variations. First, all-versus-all comparisons of the pan-genome representative proteins were conducted using Blat software (Kent, 2002). Subsequently, all genes were clustered using a broad-first-search clustering algorithm based on the alignment results: the alignments with both the identity and coverage  $>90\%$  were clustered. For each cluster, the protein with the maximum connectivity (connectivity here referring to the number of homologous genes in the cluster) was selected to be the representative "gene," and mapped to each genome assembly using Blat. The alignment results were filtered with a relatively strict cut off: identity  $>90\%$  and coverage  $>90\%$ . Then, the number of loci for which each gene could be mapped to each genome assembly was counted as the copy number of each gene in the corresponding accession. We performed Pearson correlation analysis between the copy number of each genes and its expression levels in the 33 accessions using cor.test function in R software to investigate correlation  $(P$  value  $< 0.05$  and  $|r| > 0.5)$  between gene copy number expression level.

# Inference of CNVs using short-read data

Accessions with high depth ( $>20 \times$ ) short-read resequencing data were used to detect copy number variations based on the Nipponbare genome (IRGSP1.0). We first aligned the short-read resequencing data of NIP (SRA accession: SRX734432) to the Nipponbare genome (IRGSP1.0) and filtered out the reads with mapping quality less than 30. The coverage depth of each base was calculated using the SAMtools depth function. The coverage ratio and mean depth values were then calculated using a non-overlapping 1-Kbp window. For NIP, windows with a coverage ratio over 0.75 and a mean depth within one standard deviation (STDEV) from the mean depth of the whole genome were kept for further CNV detection. For a query accession, the coverage ratio and mean depth of each 1-Kbp window were calculated, and samples with a STDEV over 1/3 of the mean depth of whole genome were abandoned due to severe sequencing bias. Finally, windows with coverage ratio over 0.75 and mean depth over three STDEV from or two-fold of the mean depth of whole genome were defined as CNVs.

# Experimental analysis of gCNV and expression level

DNA was extracted from leaves of accessions by a DNeasy Plant Mini Kit (Qigen). RNA extraction of plant materials was carried out using TRIzol (Invitrogen). qPCR experiments  $(2\times$  SYBR Green qPCR Master (Bimake) were used to verify the expression content of DNA and RNA for genes: OsVIL1, OsMADS18, Os06 g13470 and Kala4. The plant materials were list in Table S4. Primers used for qPCR were listed in Key resources table. ACTIN gene was used as the internal control.

# SV formation mechanisms

The workflow of mechanism calling in this study followed a previous study (Yang et al., 2013). According to the locations of the SV breakpoints, we divided the SVs into three groups: (1) solo SVs, for which only one SV occurred at a given site; (2) coupling SVs, exactly two SVs occurred at the same site shared one SV breakpoint; (3) more than two SVs at the same site. The detailed workflow is shown in Figures 5A, S6A, and S6B and the features of these 7 types of mechanisms were as following:

TEI: insertion, deletion or translocation was generated by the action of a single transposable element. VNTR: the generation of insertion or deletion was due to the expansion or contraction of a tandem repeat, a simple repeat, or a low complexity repeat.

NAHR: non-allelic homologous recombination,  $>200$  bp homology in the SV breakpoints. NHEJ: non-homologous end joining, 0 - 2 bp homology or 1 - 10 bp insertion in the deletion, translocation or inversion breakpoints. Alt-EJ: alternative end joining, 2 - 50 bp homology in the deletion, translocation or inversion breakpoints. SSA: single strand annealing, 50 - 200 bp homology in the deletion breakpoints. FoSTeS/MMBIR: fork stalling and template switching, template switch,  $>10$  bp deletion in the inversion or translocation breakpoints, or  $>10$  bp insertion in the deletion breakpoints.

# Graph-based genome construction

To construct a rice graph-based genome, we mapped all PAV sequences in this study to the Nipponbare genome using blot software (Kent, 2002), then filtered out the PAVs which sequence had  $>50\%$  coverage with Nipponbare genome sequence. We next conducted all-versus-all comparisons for these remaining PAVs after the preceding filtration, and then clustered these PAVs with coverage  $>50\%$  each other. We next randomly selected one PAV in each cluster for constructing a graph-based genome using the Variation graph toolkit (Garrison et al., 2018) and the Nipponbare genome as the based linear genome.

We selected 674 accessions (Table S7) from 3K-RG dataset based on sequencing depth  $>10\times$ . The phenotype data of these 674 accessions were obtained from (https://snp-seek.iri.org). In total, we obtained 5,909,051 bi-allelic SNPs with missing rate less than 0.1 and minor allele frequency over 0.02 for GWA analysis. We genotyped 47,952 SVs from the short-reads of 674 accessions using our graph-based genome and an SV genotyping pipeline integrated in Variation graph toolkit (Garrison et al., 2018) with default parameters. Both SNP-based and SV-based genome-wide association study were performed using EMMAX (v 20120210) software (Kang et al., 2010). We adopted a mixed linear model for GWAS analysis, with a principal component matrix as a fixed effect and kinship matrix as a random effect. Principle component (PC) analysis was performed using the smartPCA function in EIGENSOFT (v 5.0.2) (Reich et al., 2008). To measure the linkage of SVs with SNPs, we calculated the Pearson correlation coefficient of each SV in the graph-genome with SNPs within 500 Kbp flanking regions of the SV using in-house Perl scripts. The results of GWAS were visualized using codes based on the R package ggplot2.

# QUANTIFICATION AND STATISTICAL ANALYSIS

All details of the statistics applied in this paper are provided alongside in the respective analysis in the Method details section. Statistical analyses were performed in R 4.0.1.

# Supplemental figures

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/cd102c9d483e3c8eafdb297f2ebe54cfb5d0988bc1ed965860f326c8196036ec.jpg)  
A

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/5fb81edd3c0f553f3bf2c216c642ee9ba7ab498815a09ae5c6c0bd1a65fd11c1.jpg)  
B

C  
Figure S1. Assembly quality assessment using Bionano maps of 02428, DG, and 9311 accessions, related to Table 1  
![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/38c6adc71124ebcc99e6a4851cf4add3f2bd14e22779ecbb40f32f363974756b.jpg)  
Only 40, 32, and 109 InDels were respectively detected in the comparison between 02428 (A), DG (B), 9311 (C) assemblies and their BioNano maps.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/a6076e8fd53fc1ea55019320ae5a011cdb0ded60d19fd02fc8af77b76747b57f.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/286910694c6a2a0e389392445ba9933ff967807d83ee335932b1cdb51f22f148.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/3f320eab4057879a7db3cb308eee856f78feca89d09b6f5f73994da881fa69d1.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/a224e702be3b59cf3a0b7fcc512068577e7355d0819054aff66ef8d823d74719.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/1fc4364f37649afdb4a71a02a1883c9ac9a1ac7438bd997b3c4878dab675bfcd.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/67faabddb4b5ac3c1fa4b070b24341edd489d6487daf7fa94f2c0efb871fda73.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/d6d55bc58816911c47189e5e174c86495a59e36e910378a6485824c5cd5146e5.jpg)

Figure S2. Characterization of gene-based pan-genome and TE, related to Table 1  
![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/93663077e72362f1bee8635e498de6c8cef2428321fe328bafd269ab334305ae.jpg)  
(A) Distribution of pan-genome genes among 33 accessions. The "core" genes are those present in all accessions, "variable" genes are present in more than one but  $< 33$  accessions.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/e6b73376c5da3a3c277a4b7b610b632a2842a72f75de376e91121462cd89fef8.jpg)  
(B-D) The comparisons of the average number of total LTRs (B), Copia LTRs (C), and Gypsy LTRs (D) in accessions of the XI and GJ subpopulations.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/61c3e0647ba1bda032be8748caaaf78f65e19815786be70a7c93b1270ddde2fc.jpg)  
(E-G) The comparisons of the average length of total LTRs (E), Copia LTRs (F), and Gypsy LTRs (G) in accessions of the XI and GJ subpopulations.  
(H-J) Comparisons of the average number of total young (0 million year age) LTRs (H), young Copia LTRs (I), and young Gypsy LTRs (J) in accessions of the XI and GJ subpopulations.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/379c749d60dddb80381d3db6d9b36906659ab3ef38ccc31e2ee5b4369d7bee7a.jpg)  
A

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/2031802d53e44f20aab9e5919eac17bb226e425aac1bc7a0d0d423db785fccac.jpg)  
B  
Figure S3. Manual validations of SVs using PacBio and Hi-C datasets, related to Figure 2

(A) Example manual validations of 30 randomly selected SVs with size ranging from 2-8 Kbp (also see Table S3), based on mapping PacBio long-reads to the genome assemblies.  
(B) Example manual validations of 30 randomly selected with sizes ranging from 238 Kbp to 5.2 Mbp (also see Table S3), based on mapping the Hi-C reads to the genome assemblies at 5 Kbp resolution.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/763694e8320d9bfe761b263c280ca51b7d8218573f354bf7241be39ab8c3fc5c.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/186ef5e9b7277d6396f328aac3bb965332f0b85bfc74e11a11ee0d857abfee72.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/d99bcc4f2485a34c94cfecb4a2fa0298497cfa618b9b86a50309f5514aea1d97.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/b4aecbd372f398f3987e8af779a0520133ae9809a41a4b2e0fb7b7d861bddf86.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/5ff6a048d9eeee38bc99ce247f3b46cd2fa9cc8cb6c57d96c1f115477310e911.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/1282cefbd4105b65a74f6e841ca30a8aa99514b7cc2afe6f0e2107b06e6930cc.jpg)

Figure S4. Characterization of dSVs, related to Figure 2  
![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/4ee0257db2d5a2e953d12bd1455f1f3da6f43ecfbb94637be9c1d25120c6c2bb.jpg)  
(A) The total size of four types dSVs in each O. sativa accession.  
(B-C) Example showing how a high-quality outgroup genome assembly enabled us to confidently infer the derived status of large SVs. The Nipponbare sequence of a previously reported inversion on chromosome 6 between Nipponbare and R498 (Du et al., 2017) actually represents the derived state (B), because most O. sativa accessions and CG14 share the same state (C). The accessions with a derived state for this pericentromeric inversion among the 33 assemblies are marketed with red star.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/45daff018542e690e24de922114350225a0f2491a2d1daebeb40691c19b56538.jpg)  
$\checkmark$  stress treatment in single sample;  
P: presence of mechanical pressure stress in both samples;  
C: presence of cold stress  $(15^{\circ}\mathrm{C})$  in both samples;  
N: no stress.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/4cdab12adb5749ac761df322d886ead5d2ee5ed8709c03efb66088d1580d6eeb.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/51d9a64cf3f7cdbacc0255744f5ae47becf088de27d684c73942d592ddccb085.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/e778adeb37726e31b8847c5dcb173dca4f21b674118f879b42dde8d641a684d6.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/bb31c1ed0756c2f7acbd998c1aa6a10d4dc09ebc39169f80e5c44a62e715d6f4.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/b37ce34b71158805837569df84e3db30dbed5dc57f1cd037d05439b9389032d4.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/b8fab5b39a0cd6d1bbc9032199f987d095b40b5f46cadcdc4baa59c4c861ca48.jpg)

Figure S5. Expression characterization of dSV-gene and nonSV-gene and distributions of dSVs in terms of subpopulation, related to Figure 3

(A) Table showing the stress treatment details for each pairwise comparison in Figure 3A; only one stress condition differed per comparison.  
(B) For the same pairwise analyses in Figure 3A, Wilcoxon signed rank test based comparisons of the proportions of the dSV-genes and the nonSV-genes with the indicated FPKM fold change levels.  
(C) The distribution of expressed (FPKM > 1) dSV-genes and nonSV-genes in R527 accession across 29 RNA sequencing samples from R527.  
(D) The expression level comparisons between dSV-genes and nonSV-gene of R527 accession in the 29 RNA sequencing samples from R527.  $(^{**}p < 0.0001$ , Wilcoxon signed rank.)  
(E) Examples of dSVs respectively overlapping upstream, coding region, intron, or downstream sequences that are significantly associated with altered expression of the corresponding genes (\*\*: p < 0.001, Student's t test).  
(F) The distribution of all dSVs in this study in terms of four main  $O$ . sativa subpopulations.  
(G) The distribution in 9 subpopulations for 5,393 fixed dSVs (present in all accessions of a given subpopulation). 2,535 dSVs are fixed in a single subpopulation.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/5f2a226782ceda514297ea072c49cd340fff5e96581e36890d2d6715e5b21b53.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/2ea0d6626fe195ca60acf66f78019660a2d786159d4fc14c356473af344a6ecc.jpg)

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/ce7a0dfd4dd0b3939073f1b7d6b6085163facd71556aa22ef9c8071c260c6277.jpg)  
Figure S6. Flowchart for assigning mechanisms for translocations and inversions, and characterization of SV borders in terms of TEs, related to Figure 5

(A-B) This flowchart shows how breakpoint features were used to assign mechanisms for translocations (A) and inversions (B). Based on the flowchart from a previous study (Yang et al., 2013).  
(C) The percentage of borders which overlapped with TEs in terms of the four indicated types of SVs.

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/bae7500fd1d6d4cd5639b6cf0dee53d2713a65dd83ff8e0e7d12cc2b5f6a8831.jpg)  
A  
PAV size

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/63b586e6e264af6cd2f0315187c1ca6cd019887c35c0f23215d9b0583cf19894.jpg)  
B

![](https://cdn-mineru.openxlab.org.cn/result/2025-11-19/6cd32bf2-5171-492b-b591-cff3f2f9999d/ff5cf38ae44e06eaf68b5617c88578700ab265b07e4233789f2e221e8a267739.jpg)  
C  
Figure S7. Characterization of PAVs based on the graph-based genome, related to Figure 6

(A) Histogram the size distribution of the PAVs identified using based on mapping the short-reads data for 674 accessions from the 3K-RG dataset to our graph-based genome.  
(B) Comparison of distribution pattern between two sets of PAVs among O. sativa subpopulations: PAVs genotyped from the short-reads of 674 accession using graph-based genome, and PAVs from 31 assemblies in this study using Nipponbare assembly as reference genome. These similar patterns indicate no obvious subpopulation biases for the PAVs based on the graph-based genome.  
(C) The distribution of the SV associated with early leaf senescence among subpopulations.