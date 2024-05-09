# MCNP-OutputProcessing

MCNP输出文件的处理，根据内部的不同cell分割处理多个子文件思路为：
从第一个cell +“序列”为开始，到最后一个关键字total为结束分割数据把关键信息保留，导入成struct下的多个字段，每个字段对应要处理的一个文件，字段之下会分成各个文件中要分隔的探测器“cell”单元。

使用时请先将.o的输出文件放置在output的文件夹下，将代码中的文件路径改写到output文件夹，运行.mlx文件一键处理。

第二段生成矩阵数据未完全写完，故注释。

