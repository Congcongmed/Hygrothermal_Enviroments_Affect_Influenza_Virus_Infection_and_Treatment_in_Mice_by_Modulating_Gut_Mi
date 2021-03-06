File Structure of Results
|--Large project number_subproject code/
|   |--Clean_Data/                                 [High quality data filtered from raw data]
|   |   |--Sample_Name
|   |   |   |--*_1.fq.gz                           [Clean Data read1]
|   |   |   |--*_2.fq.gz                           [Clean Data read2]
|   |   |-CleanData_stat.xls                       [Statistics excel sheet of Clean Data]
|   |--Connect_Tags/                               [Tags connected of PE reads]
|   |   |--*.Tags.fasta.gz                         [Fasta file of Tags]
|   |   |--ConnectTags_stat.xls                    [Statistics excel sheet of Tags]
|   |--OTU_Cluster_Taxonomy/                       [OTU analysis result]
|   |   |--1.OTU_Cluster_Taxonomy/                 [OTU clustering and its annotation file]
|   |   |   |--OTU_final.fasta                     [Fasta file of OTU represented tags]
|   |   |   |--OTU_taxonomy.xls                    [Statistics of OTU taxonomy]
|   |   |   |--OTU_table_for_biom.txt              [Statistics of OTU taxonomy and its abundance of each sample]
|   |   |   |--OTU.shared.xls                      [Statistics of OTU abundance of each sample] 
|   |   |   |--OTU_stat_detail.xls                 [Detailed statistics excel sheet of OTU]
|   |   |   |--OTU_final_phylogeny_tree.txt        [TXT file of OTU phylogeny tree]
|   |   |--2.OTU_Analysis/                         [OTU analysis]
|   |   |   |--*venn.png                           [Venn diagram for OTU]
|   |   |   |--*sharedOTU.venn.xls                 [Statistics of common and specific OTU ID among samples or groups]
|   |   |   |--OTU_PCA_*.pdf                       [Figure of PCA for OTU]
|   |   |   |--*PCA.coordinate.xls                 [PCA coordinates of samples]
|   |   |   |--*.OTU_rank.pdf                      [Figure of OTU rank]
|   |   |   |--genus.OTU.fasta                     [Fasta file of unique tags representing genus]
|   |   |   |--genus.phylogeny.tree                [Phylogeny tree in newick format at the level of genus]
|   |   |   |--genus.tree.pdf                      [Figure of Phylogeny tree at the level of genus]
|   |   |--3.Taxa_summary/                         [Summary file of species annotation]
|   |   |   |--*.absolute_abundance.xls            [Statistics excel sheet of reads number of each species at different taxonomic level]
|   |   |   |--*_relative_abundance.xls            [Statistics excel sheet of species relative abundance at different taxonomic level]
|   |   |   |--*_taxonomy_barplot.pdf              [Species annotation histogram at different taxonomic level]
|   |   |--4.Species_heatmap/                      [Heat map for species]
|   |   |   |--*.relative_abundance_log10.xls      [Statistics of species relative abundance at different taxonomic level(log10 value)]
|   |   |   |--*.heatmap.pdf                       [Species heat map at different taxonomic level]
|   |--Alpha_Diversity/                            [Summary of Alpha diversity]
|   |   |--Alpha_diversity.xls                     [Calculation result of Alpha diversity indexes]
|   |   |--Alpha_diversity.detail.xls              [Detailed calculation result of Alpha diversity indexes]
|   |   |--*.Alpha.xls                             [Calculation result of Alpha diversity indexes with sampling]
|   |   |--observed_species.Rarefaction.pdf        [Figure of rarefaction curve with observed_species value]
|   |   |--chao.Rarefaction.pdf                    [Figure of rarefaction curve with chao value]
|   |   |--ace.Rarefaction.pdf                     [Figure of rarefaction curve with ace value]
|   |   |--shannon.Rarefaction.pdf                 [Figure of rarefaction curve with shannon value]
|   |   |--simpson.Rarefaction.pdf                 [Figure of rarefaction curve with simpson value]
|   |   |--*Alpha.boxplot.pdf                      [Boxplot of Alpha diversity of different groups]
|   |   |--*Alpha.test.result.xls                  [Rank sum test of Alpha diversity of different groups]
|   |--Beta_Diversity/                             [Summary of Beta diversity]
|   |   |--Beta_diversity_index/
|   |   |   |--*_Beta_diversity.txt                [Statistics of Beta diversity]
|   |   |   |--*_diversity_heatmap.pdf             [Heat map for Beta diversity]
|   |   |   |--*.tree.pdf                          [Figure of clustering]
|   |   |   |--*.jackknife_named_nodes.tree        [Figure of clustering in Newick format]
|   |   |   |--2d_plots/*                          [2d plot of PCoA]
|   |   |   |--2d_plots/*                          [3d plot of PCoA]
|   |--Diff_Analysis                               [Difference analysis result between the groups]
|   |   |--Test_method
|   |   |   |--Phylum/                             [Difference analysis result at phylum level]
|   |   |   |--Class/                              [Difference analysis result at class level]
|   |   |   |--Order/                              [Difference analysis result at order level]
|   |   |   |--Family/                             [Difference analysis result at family level]
|   |   |   |--Genus/                              [Difference analysis result at genus level]
|   |   |   |--Species/                            [Difference analysis result at species level]
