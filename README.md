Hi ALL：

Data_processing_assistant_for_JJM是一个数据处理助手，它可以用来处理CP、FT、可靠性数据，目的是用来提高数据处理效率。
1. 对于CP数据，该助手可以提取良率、画概率分布图（选择By wafer或者By lot）、画正态分布图同时计算cp cpk（该功能目前不成熟）、画Map、输出PPT。
2. 对于FT数据，该助手可以画概率分布图、画正态分布图同时计算cp cpk（该功能目前不成熟）、输出PPT。
3. 对于可靠性数据，该助手可以画趋势图、概率分布图。
使用时请注意：在公盘中将数据解密后再进行处理！！！

版本V1.0.0 

该助手目前可以实现的功能如下：
1. CP map				----用来画CP数据的map。
通过raw_data_by_wafer.py--->merge_BIN.py--->BIN_map.py的顺序运行脚本文件。

2. CP probability		----用来画CP数据的概率分布图，同时可以选择是否生成正态分布图和输出PPT。
通过raw_data_by_wafer.py(按照wafer来处理数据)/raw_data_by_lot.py(按照lot来处理数据)--->merge_BIN.py--->probability.py的顺序来运行脚本文件。

3. FT probability		----用来画FT数据的概率分布图，同时可以选择是否生成正态分布图和输出PPT。
通过raw_data_of_FT.py--->merge_BIN.py--->probability.py的顺序来运行脚本。

4. reliability			----用来画可靠性数据的趋势图和概率分布图
4.1 Reliability probability distribution graph   ----可靠性数据的概率分布图
通过manage_data_for_probability.py--->merge_BIN.py--->probability.py的顺序来运行脚本文件。
4.2 Reliability Trend Chart		----可靠性数据的趋势图
通过reliability_merge_data.py--->reliability_draw_picture.py的顺序来运行脚本文件。

（后续版本更新介绍可以浏览README.md文件）

Best Regard
LYX