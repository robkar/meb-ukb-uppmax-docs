# UK Biobank genotype data

This file describes the set of UK Biobank genotype data currently available in
the Uppmax/bianca project sens2017519 ("AGE"), PI Sara Hägg.

The genotype data was released in 2017 and is thoroughly described in [The UK
Biobank resource with deep phenotyping and genomic data (Bycroft et al.
2018)](https://www.nature.com/articles/s41586-018-0579-z)

## Raw source data

As downloaded from UKB, located in folder `/proj/sens2017519/nobackup/b2016326_nobackup/UKBB/`

The file sets in this folder are described in more detail in
[ukb_genetic_data_description.txt](ukb_genetic_data_description.txt), with an
overview presented below: 

**Genotype calls** ([plink format](https://www.cog-genomics.org/plink/1.9/formats#bed))
|||
|---|---|
|Calls BED|			ukb_cal_chrN_v2.bed|
|Calls BIM|			ukb_snp_chrN_v2.bim|
|Calls FAM|			ukbA_cal_v2_sP.fam|

**Imputation files** ([BGEN format](https://www.well.ox.ac.uk/~gav/bgen_format/spec/v1.2.html))
|||
|---|---|
|Imputation BGEN|			ukb_imp_chrN_v3.bgen|
|Imputation BGI|		ukb_imp_chrN_v3.bgen.bgi|
|Imputation MAF+info|		ukb_mfi_chrN_v3.txt|
|Imputation sample chr1-22|	ukbA_imp_chrN_v3_sP.sample|
|Imputation sample chrX	|	ukbA_imp_chrX_v3_sP.sample|
|Imputation sample chrXY	|	ukbA_imp_chrXY_v3_sP.sample|
|Haplotypes BGEN|			ukb_hap_chrN_v2.bgen	|
|Haplotypes BGI|			ukb_hbg_chrN_v2.bgi|
|HLA Imputation|			ukb_hla_v2.txt|

**Raw data for CNV calling and genotype cluster plots**
|||
|---|---|
|CNV log2r|			ukb_l2r_chrN_v2.txt|
|CNV baf|				ukb_baf_chrN_v2.txt|
|Intensity|			ukb_int_chrN_v2.bin|

**Various sample and SNP metadata**
|||
|---|---|
|Marker-QC|			ukb_snp_qc.txt|
|Sample-QC|			ukb_sqc_v2.txt|
|Relatedness|			ukbA_rel_sP.txt|
|Confidences|			ukb_con_chrN_v2.txt|
|SNP-posterior|			ukb_snp_posterior_chrN.bin|
|Batch|				ukb_snp_posterior.batch|
|SNP-posterior chrX BIM|		ukb_snp_posterior_chrX_haploid.bim|

Wildcards in filenames:
- N: chromosome label (1..22,X,Y,XY,MT)
- P: number of consenting participants
- A: researchers UK Biobank application ID (22224)

See also <https://www.ukbiobank.ac.uk/enable-your-research/about-our-data/genetic-data> and <https://biobank.ndph.ox.ac.uk/ukb/label.cgi?id=100314>

## Raw data updates

Note that when participants withdraw from the UK Biobank, new `.fam` and
`.sample` files are generated with their ID replaced with a negative number, and
the sample count in the filename updated. Please use the most up-to-date files
for any in-progress analyses (but we keep the older files so older analyses can
be reproduced).

## Derived data

Derived data and format conversions shared with all users: [NONE YET]
