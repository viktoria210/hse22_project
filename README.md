# hse22_project
Целью работы над проектом является поиск и изучение консервативных участков генома Z-ДНК в геномах прокариот и эукариот, где . В процессе выполнения проекта будут получены важные практические навыки биоинформатика -- работа в командной строке с утилитой bedtools, визуализация данных, конвертация координат участков между разными версиями генома (разными организмами) и т.п.

**таксон**: Actinobacteria  
**род**: Bifidobacterium 

**Геномы**: 
- Bifidobacterium actinocoloniiforme DSM 22766 chromosome  (Bifidobacterium actinocoloniiforme)
- Bifidobacterium angulatum DSM 20098 = JCM 7096 chromosome (Bifidobacterium angulatum)
- Bifidobacterium animalis subsp. lactis BLC1 (Bifidobacterium animalis)
- Bifidobacterium catenulatum DSM 16992 = JCM 1194 = LMG 11043 strain JCM 1194 chromosome (Bifidobacterium catenulatum )
- Bifidobacterium pseudolongum strain UMB-MBP-01 chromosome (Bifidobacterium pseudolongum)

[Ссылка на Google Colab](https://colab.research.google.com/drive/1nPwuXqnlYLaghuUytmimn0YXrnsKLu0f?usp=sharing)

## Таблица

|Название вида                        |Количество хромосом| Количество аннотированных генов | доля аннотированных генов в геноме |Длина генома (bp)  | Кол-во участков Z-DNA* |Кол-во участков Z-DNA** |Общая длина участков с zh_score > 500|
|:------------------------------------|:------------------|:--------------------------------|:-----------------------------|:-------------------|:------------------------|:--------------------------|:----------------|
|Bifidobacterium animalis             | 1                 | 1457                            | 75.49                        |1938583             |1938583                  |27687                      |153744|
|Bifidobacterium angulatum            | 1                 | 1684                            | 98.0483                      |2021974             |2021974                  |19073                      |172160|
|Bifidobacterium catenulatum          | 1                 | 1549                            | 86.5511                      |2079525             |2079525                  |17128                      |279588|
|Bifidobacterium actinocoloniiforme   | 1                 | 1558                            | 86.4118                      |1830060             |1830060                  |15248                      |194776|
|Bifidobacterium pseudolongum         | 1                 | 1640                            | 87.7742                      |2008102             |2008102                  |53153                      |536610|

 '*' - Количество ***предсказанных*** участков Z-DNA с помощью программы ***Z-HUNT***.

 '**' - * с ZH-score > 500
 
 ## Гистограммы значений zh-score для всех геномов, полученных с помощью Zhunt
![image](https://user-images.githubusercontent.com/60792064/173845842-d039b442-68a6-4071-9df3-e0361d31087a.png)
![image](https://user-images.githubusercontent.com/60792064/173845883-5856714e-6025-4c66-8359-395d8ebcfd7a.png)
![image](https://user-images.githubusercontent.com/60792064/173845901-37dfa1f0-c5a9-4115-a205-b12712d20196.png)
![image](https://user-images.githubusercontent.com/60792064/173845922-a0da3520-8b18-48da-9b58-c8906d56d49d.png)
![image](https://user-images.githubusercontent.com/60792064/173845950-c06bd01f-45f8-48e2-a60f-f73cda3f128d.png)

## Полученные гомологичные кластеры
![image](https://user-images.githubusercontent.com/60792064/173872594-ac425bb2-baaa-4649-ab19-726314ae1d61.png)
![image](https://user-images.githubusercontent.com/60792064/173872616-7fe237fa-e1b0-44fd-bf17-a09d5975137a.png)

## Полученные кластеры и количество элементов в них
|Количество генов|Количетво Z-dna|
|:---------------|:--------------|
|0               |    1581       |

Таким образом можем наблюдать только один кластер, в котором объекты объединены отсутствием левозакрученной спирали.

>AEN76886.1 hypothetical protein BLC1_1112 [Bifidobacterium animalis subsp. lactis BLC1]
>AEN77261.1 DedA family protein [Bifidobacterium animalis subsp. lactis BLC1]
>AEN75865.1 FHA domain protein [Bifidobacterium animalis subsp. lactis BLC1]
>AEN75898.1 NAD-dependent epimerase/dehydratase [Bifidobacterium animalis subsp. lactis BLC1]
>AEN76745.1 Ppx/GppA phosphatase family protein [Bifidobacterium animalis subsp. lactis BLC1]
>AEN76146.1 50S ribosomal protein L3 [Bifidobacterium animalis subsp. lactis BLC1]
>AEN77230.1 sulfatase [Bifidobacterium animalis subsp. lactis BLC1]
>AEN76238.1 HAD-superfamily hydrolase [Bifidobacterium animalis subsp. lactis BLC1]
>AEN76534.1 ribulose-phosphate 3-epimerase [Bifidobacterium animalis subsp. lactis BLC1]
>AEN76798.1 putative DNA recombination-mediator protein A [Bifidobacterium animalis subsp. lactis BLC1]

|Количество генов в кластере |Гены                  |Функции генов                |
|:---------------------------|:---------------------|:----------------------------|
| 5                           |AEN76886.1            |hypothetical protein BLC1_1112|
| 5                           |AEN77261.1            |DedA family protein|
| 5                           |AEN75865.1            |FHA domain protein|
| 2                           |AEN75898.1            |NAD-dependent epimerase/dehydratase|
| 5                           |AEN76745.1            |Ppx/GppA phosphatase family protein|
| 5                           |AEN76146.1            |50S ribosomal protein L3 |
| 4                           |AEN77230.1            |sulfatase  | 
| 2                           |AEN76238.1            |HAD-superfamily hydrolase |
| 5                           |AEN76534.1            |ribulose-phosphate 3-epimerase |
| 5                           |AEN76798.1            |putative DNA recombination-mediator protein A |

## Aссоциирования Z-DNA с генами
**Bifidobacterium actinocoloniiforme**
![image](https://user-images.githubusercontent.com/60792064/173954479-235d2940-d294-494b-a596-19429d038317.png)
**Bifidobacterium angulatum**
![image](https://user-images.githubusercontent.com/60792064/173954496-b9e244ca-0168-4aee-911d-3c9594e30865.png)
**Bifidobacterium animalis**
![image](https://user-images.githubusercontent.com/60792064/173954549-78aceddf-3ee5-4f18-9a6d-277ba9f2978e.png)
**Bifidobacterium catenulatum**
![image](https://user-images.githubusercontent.com/60792064/173954589-c85e0764-0958-4525-8f23-f82fb91c5a72.png)
**Bifidobacterium pseudolongum**
![image](https://user-images.githubusercontent.com/60792064/173954605-e405cc4c-103d-44cf-9c52-9811f20a24b2.png)

## G-Квадруплексы
|    | Название           |   Количество предсказанных G-квадруплексов |   Общая длина G-квадруплексов |
|---:|:-------------------|-------------------------------------------:|------------------------------:|
|  0 | animalis           |                                         42 |                          1018 |
|  1 | angulatum          |                                         39 |                           904 |
|  2 | catenulatum        |                                         15 |                           355 |
|  3 | actinocoloniiforme |                                        209 |                          4909 |
|  4 | pseudolongum       |                                         36 |                           872 |

![image](https://user-images.githubusercontent.com/60792064/173955042-ad2842ab-2d7f-4669-a9af-d4f9fa4800c9.png)
![image](https://user-images.githubusercontent.com/60792064/173955056-cd89a399-21eb-4c7a-a87c-9d766fa734ca.png)
![image](https://user-images.githubusercontent.com/60792064/173955075-8bffa6a5-ac70-4894-8ff7-d01ad32e30f3.png)
![image](https://user-images.githubusercontent.com/60792064/173955086-04b0d746-b64e-49ce-bba1-34e11938ae5c.png)
![image](https://user-images.githubusercontent.com/60792064/173955094-4c179720-15d5-4c93-8021-5b15cc82ef4c.png)

Можем наблюдать давольно большое количество предсказанных G-квадруплексов в целом. Однако консервативность не наблюдаем, как и в ситуации с Z-DNA. 

==> quad_intersect_animalis.bed <==

==> quad_intersect_angulatum.bed <==

==> quad_intersect_catenulatum.bed <==

==> quad_intersect_actinocoloniiforme.bed <==

==> quad_intersect_pseudolongum.bed <==
