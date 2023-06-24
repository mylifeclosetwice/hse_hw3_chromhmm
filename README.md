# Домашнее задание 3
Ссылка на тетрадку: https://colab.research.google.com/drive/1E21O3-jw5cdV7gvPggCg3YIit-Dk_OOH?usp=sharing
## Данные:
Клеточная линия: K562
### 10 гистоновых меток

Num	| Histone mark |	File name 
:-------------------------:|:-------------------------:|:-------------------------:
1 | H3k4me1 | wgEncodeBroadHistoneK562H3k4me1StdAlnRep1.bam
2 | H3k27ac | wgEncodeBroadHistoneK562H3k27acStdAlnRep1.bam
3 | H3K79me2 | wgEncodeBroadHistoneK562H3k79me2StdAlnRep1.bam
4 | H4K20me1 | wgEncodeBroadHistoneK562H4k20me1StdAlnRep1.bam
5 | H3K9me3 | wgEncodeBroadHistoneK562H3k9me3StdAlnRep1.bam
6 | H3k9me1 | wgEncodeBroadHistoneHuvecH3k9me1StdAlnRep1.bam
7 | H3K27me3 | wgEncodeBroadHistoneK562H3k27me3StdAlnRep1.bam
8 | H2AFZ | wgEncodeBroadHistoneK562H2azStdAlnRep1.bam
9 | H3k9ac | wgEncodeBroadHistoneK562H3k9acStdAlnRep1.bam
10 | H3k4me2 | wgEncodeBroadHistoneK562H3k4me2StdAlnRep1.bam

Контрольный файл: wgEncodeBroadHistoneK562ControlStdAlnRep1.bam


## ChromHMM-выдача:
Emission	| Transition |	Overlap 
:-------------------------:|:-------------------------:|:-------------------------:
![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/1816a2e9-ac56-45b6-96aa-0dbcaa6a1f4a) | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/2fc68dd9-5dc6-47a1-bbfe-241c195b5615) | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/73f6470e-8fa6-4894-b7f5-27be48a93856) 

RefSeqTSS	| RefSeqTES
:-------------------------:|:-------------------------:
![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/037c46ec-4e80-4777-8404-0e35f6547a44) | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/adda044e-cb8a-4b47-95b9-d3ce885c130b)




## Эпигенетические типы:
CpGIsland
RefSeqExon
RefSeqTSS
RefSeqTSS2kb
RefSeqGene
RefSeqTES
laminB1lads
State | Name | Localisation | Marks | Picture
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
1 | Transcribed | Появляется преимущественно в RefSeqGene | Для состояния характерна метка H3K79me2
2 | Transcribed | Появляется преимущественно в RefSeqGene, реже в RefSeqTSS2kb и RefSeqTES | Для состояния характерны метки H3K79me2 и H3k4me1, менее характерны метки H4K20me1, H3k27ac, H3k9ac и H3k4me2
3 | Transcribed | Появляется преимущественно в RefSeqTES, реже в RefSeqExon, RefSeqTSS2kb и laminB1lads | Для состояния характерна метка H3k4me1 , менее характерна метка H3k27ac
4 | Enhancer | Появляется преимущественно в RefSeqTES, реже в RefSeqGene, RefSeqExon, RefSeqTSS2kb и laminB1lads | Для состояния характерны метки H3k4me1, H2AFZ, H3k27ac, H3k9ac и H3k4me2
5 | Active promoter | Появляется преимущественно в CpGIsland, RefSeqExon, RefSeqTSS и RefSeqTSS2kb, реже в RefSeqTES. Сконцентрировано около TSS | Для состояния характерны метки H2AFZ, H3k27ac, H3k9ac и H3k4me2, менее характерна метка H3k4me1
6 | Promoter | Появляется преимущественно в RefSeqExon, RefSeqTES, RefSeqTSS2kb, реже в CpGIsland, RefSeqGene и RefSeqTSS | Для состояния характерны метки H3K79me2, H3k27ac, H3k9ac и H3k4me2, менее характерны метки H3k4me1 и H2AFZ
7 | Enhancer | Появляется преимущественно в laminB1lads реже в RefSeqTES, CpGIsland, RefSeqExon, RefSeqTSS2kb и RefSeqTSS | Для состояния характерна метка H3k4me1 и H2AFZ
8 | Enhancer| Появляется преимущественно в RefSeqTES, реже в RefSeqExon, RefSeqGene и laminB1lads | Для состояния нет характерных меток 
9 | Repressed | Появляется преимущественно в laminB1lads | Для состояния нет характерных меток
10 | Heterochromatin | Появляется преимущественно в laminB1lads, реже в RefSeqTES, RefSeqGene и RefSeqExon | Для состояния характерна метка H3K27me3 (но и для нее вероятность крайне мала)
 
