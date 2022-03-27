# hse_hw3_chromhmm
## Бордюгов Максим

[colab](https://colab.research.google.com/drive/11xwyp15Ofi3T6uHYlRRqOrPsO6LoJir-?usp=sharing)

| №|метка   |файл             |                                           оригинал|
|---:|:-----|:----------------|--------------------------------------------------:|
| 1|H3k27ac |bams/H3k27ac.bam | wgEncodeBroadHistoneA549H3k27acDex100nmAlnRep1.bam|
| 2|H3k27me3|bams/H3k27me3.bam|wgEncodeBroadHistoneA549H3k27me3Dex100nmAlnRep1.bam|
| 3|H3k36me3|bams/H3k36me3.bam|wgEncodeBroadHistoneA549H3k36me3Dex100nmAlnRep1.bam|
| 4|H3k04me1|bams/H3k04me1.bam|wgEncodeBroadHistoneA549H3k04me1Dex100nmAlnRep1.bam|
| 5|H3k04me2|bams/H3k04me2.bam|wgEncodeBroadHistoneA549H3k04me2Dex100nmAlnRep1.bam|
| 6|H3k04me3|bams/H3k04me3.bam|wgEncodeBroadHistoneA549H3k04me3Dex100nmAlnRep1.bam|
| 7|H3k79me2|bams/H3k79me2.bam|wgEncodeBroadHistoneA549H3k79me2Dex100nmAlnRep1.bam|
| 8|H3k09ac |bams/H3k09ac.bam |   wgEncodeBroadHistoneA549H3k09acEtoh02AlnRep1.bam|
| 9|H3k09me3|bams/H3k09me3.bam|  wgEncodeBroadHistoneA549H3k09me3Etoh02AlnRep1.bam|
|10|H4k20me1|bams/H4k20me1.bam|  wgEncodeBroadHistoneA549H4k20me1Etoh02AlnRep1.bam|
|  |Control |bams/Control.bam | wgEncodeBroadHistoneA549ControlDex100nmAlnRep1.bam|

[cellmarkfiletable.txt](res/cellmarkfiletable.txt)

```txt
A549	H3k27ac	bams/01_H3k27ac.bam	bams/Control.bam
A549	H3k27me3	bams/02_H3k27me3.bam	bams/Control.bam
A549	H3k36me3	bams/03_H3k36me3.bam	bams/Control.bam
A549	H3k04me1	bams/04_H3k04me1.bam	bams/Control.bam
A549	H3k04me2	bams/05_H3k04me2.bam	bams/Control.bam
A549	H3k04me3	bams/06_H3k04me3.bam	bams/Control.bam
A549	H3k79me2	bams/07_H3k79me2.bam	bams/Control.bam
A549	H3k09ac	bams/08_H3k09ac.bam	bams/Control.bam
A549	H3k09me3	bams/09_H3k09me3.bam	bams/Control.bam
A549	H4k20me1	bams/10_H4k20me1.bam	bams/Control.bam
```

- __Emission__  
  ![](img/1.png)
- __Transition__  
  ![](img/2.png)
- __Overlap__  
  ![](img/3.png)
- __RefSeqTSS__  
  ![](img/4.png)
- __RefSeqTES__
  ![](img/5.png)

### 1 = __Heterochromatin__
![](img/state01.png)
### 2 = __Repressed__
![](img/state02.png)
### 3 = **Weak_Txn**
![](img/state03.png)
### 4 = **Weak_Txn**
![](img/state04.png)
### 5 = **Weak_Txn**
![](img/state05.png)
### 6 = **Weak_Enhancer**
![](img/state06.png)
### 7 = **Weak_Enhancer**
![](img/state07.png)
### 8 = **Strong_Enhancer**
![](img/state08.png)
### 9 = **Active_Promoter**
![](img/state09.png)
### 10 = **Active_Promoter**
![](img/state10.png)

__Вывод__: по данные графикам, можно предположить гистоновую модификацию по типу

_Пример_: `state08` выражен для следующих модификаций:
- `H2A.Z`
- `H3K4m1`
- `H3K4m2`
- `H3K4m3`
- `H3K4m1`
- `H3K9ac` _(слабо)_
- `H3K27ac`

## Бонус
[colab](https://colab.research.google.com/drive/11xwyp15Ofi3T6uHYlRRqOrPsO6LoJir-?usp=sharing)