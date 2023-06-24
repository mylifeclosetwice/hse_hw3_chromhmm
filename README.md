![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/ec3816f5-fd18-4e6c-9eae-896213fb2aec)![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/9fc7a26a-d34b-4083-934e-069472d24119)# Домашнее задание 3
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
1 | Transcribed | Появляется преимущественно в RefSeqGene | Для состояния характерна метка H3K79me2 | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/c4ea1213-6c06-42f3-8b70-dc76f945515e)

2 | Transcribed | Появляется преимущественно в RefSeqGene, реже в RefSeqTSS2kb и RefSeqTES | Для состояния характерны метки H3K79me2 и H3k4me1, менее характерны метки H4K20me1, H3k27ac, H3k9ac и H3k4me2 | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/d53e62f0-cd0e-4091-872d-80f82643366f)

3 | Transcribed | Появляется преимущественно в RefSeqTES, реже в RefSeqExon, RefSeqTSS2kb и laminB1lads | Для состояния характерна метка H3k4me1 , менее характерна метка H3k27ac | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/a50614d1-c305-4697-92af-b8fc01ee0a21)

4 | Enhancer | Появляется преимущественно в RefSeqTES, реже в RefSeqGene, RefSeqExon, RefSeqTSS2kb и laminB1lads | Для состояния характерны метки H3k4me1, H2AFZ, H3k27ac, H3k9ac и H3k4me2 | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/bd789cae-f8ec-4dd6-b11c-96271c6233c2)

5 | Active promoter | Появляется преимущественно в CpGIsland, RefSeqExon, RefSeqTSS и RefSeqTSS2kb, реже в RefSeqTES. Сконцентрировано около TSS | Для состояния характерны метки H2AFZ, H3k27ac, H3k9ac и H3k4me2, менее характерна метка H3k4me1 | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/28c140de-8945-4937-8340-494bf2f251e1)

6 | Promoter | Появляется преимущественно в RefSeqExon, RefSeqTES, RefSeqTSS2kb, реже в CpGIsland, RefSeqGene и RefSeqTSS | Для состояния характерны метки H3K79me2, H3k27ac, H3k9ac и H3k4me2, менее характерны метки H3k4me1 и H2AFZ | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/d4e4b76c-ca39-4afd-a477-c6e2bf8656e9)

7 | Enhancer | Появляется преимущественно в laminB1lads реже в RefSeqTES, CpGIsland, RefSeqExon, RefSeqTSS2kb и RefSeqTSS | Для состояния характерна метка H3k4me1 и H2AFZ | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/b2d32ec6-46b5-4808-afb9-2672696ab4e9)

8 | Enhancer| Появляется преимущественно в RefSeqTES, реже в RefSeqExon, RefSeqGene и laminB1lads | Для состояния нет характерных меток | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/c91faf5f-85f3-4eb3-b930-58766e2c9221)

9 | Repressed | Появляется преимущественно в laminB1lads | Для состояния нет характерных меток | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/08e3361e-387a-4262-8c23-7420ad2371ea)

10 | Heterochromatin | Появляется преимущественно в laminB1lads, реже в RefSeqTES, RefSeqGene и RefSeqExon | Для состояния характерна метка H3K27me3 (но и для нее вероятность крайне мала) | ![image](https://github.com/mylifeclosetwice/hse_hw3_chromhmm/assets/71773580/2f59d709-b6ba-466c-8d4a-e3020289ebed)

 
