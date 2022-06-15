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

