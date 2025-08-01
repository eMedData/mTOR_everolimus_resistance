#This repository contains scripts pertaining to "Systems analysis links SMARCD3 regulons to alternate growth signaling and mEK inhibitor response in everolimus-resistant breast cacner cells".

#Each script has its own libraries at the top of the script that are used to run the code.

#The input file for "01_filter.normalize_everSamples.Rmd" is "COH069_15929R_data.counts.txt", which contains the raw counts for the cell line samples. This script generates the filered/normalized counts used for downstream analyses. 
#"02_DEGs_lmeModel.Rmd" uses the output counts file generated above to identify differentially expressed genes (DEGs) between senstive and resistant cells.
#"03_ssGSEA.Rmd" runs ssGSEA using output counts file to generate ssGSEA scores for the samples.
#The file containing ssGSEA scores is used in "04_lmeModel_ssGSEA_Scores.Rmd" to identify differentially enriched gene-sets between sensitive and resistant cells.
#The meta-phenotype analysis described in figures 2B and 2D in the manuscript can be reproduced using the script titled "05_metaPhenotypesAnalysis.Rmd".
#"5.1_databaseReceptorLigandPairs.Rmd" script uses the database frome Ramilowski et al. 2015 to identify ligand/receptor pairs pertaining to figures S5A and S5B. 
#"06_complexheatmap_figures.Rmd" generates heatmaps of differentially expressed gene-sets pertaining to figures 2A and 2C in the manuscript.
#"07_StructureCountForARACNe.Rmd" perpares the counts for ARACNe-AP and "09_Viper.Rmd" runs regulon enrichment pertaining to figures 3 and S6 in the manuscript.
#The script titled "10_Sabine_et_al_analysis" runs code for the clinical dataset described in the manuscript.
#"11_SMARCD3ResistanceRegulonSignatureInSen.EverRCells.Rmd" measures reglon activity in cell line samples, as described in figure 4B of the manuscript.
#The scripts titled "12_gdsc_microarray_auc_processesing_mr_phenotype_drug_sensitivity_ssGSEA_AUC_data.Rmd" and "13_gdsc1_aucImpute_PearsonCorr_plots.Rmd" run code that uses the GDSC pharmacogenomics datasets to identify anti-cancer drugs against the SMARCD3 regulon signatures shown in figure 5 of the manuscript.
#"14_normalize_ccle_RNAseq_counts_v2.Rmd", "15_ccle_ctrp_v1_save_Files_PredictiveModel_v2.Rmd", "16_ccle_ctrp_v1_pearsonCorAnalysis.Rmd", "17_ccle_ctrp_v2_save_Files_PredictiveModel_v2.Rmd", "16_ccle_ctrp_v1_pearsonCorAnalysis.Rmd" and "18_ccle_ctrp_v2_pearsonCorAnalysis.Rmd" are scripts used to identify anti-cancer drugs with the CCLE/CTRP version 1 and version 2 pharmacogenomics datasets.
The SMARCD3 RNAi data from Jordan et al. 2013 was leveraged to understand SMARCD3 modulation (figure S7). This analysis can be run using the "19_smarcd3_RNAi_analysis.Rmd" script.
The SWI/SNF inhibitor treated samples leveraged from Xiao et al. 2022 and Martin et al. 2023 can be found in "20_swi:snf_inhibitors_datasets.Rmd"

R version 4.4.2 (2024-10-31) -- "Pile of Leaves" was used for all analyses.

