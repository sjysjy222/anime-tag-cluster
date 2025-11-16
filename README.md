# anime-tag-cluster

数据来自https://bangumi.tv/anime
基于UMAP算法与标签标记数的泛百合动画聚类图。

通过bangumi网页端获取动画排行榜上所有项目号码，再用项目号从bangumi官方api https://bangumi.github.io/api/ 获取项目tag及其标注数，
随后用ln(1+x)压缩标注数，并用UMAP方法将高维矩阵压缩至2维。最后使用Kmeans方法对二维矩阵上的点聚类。

使用Anime下拉菜单可选择具体动画及其相邻的10部动画。
使用Tag下拉菜单可选择具体动画标签。
建议使用PC端查看。

代码位于Bangumi_tag_umap_ver2.ipynb

在release中可以找到所有动画，及百合动画聚类的源文件

示例html:

动画聚类：https://sjysjy222.github.io/anime-tag-cluster/full_anime

百合聚类：https://sjysjy222.github.io/anime-tag-cluster/


