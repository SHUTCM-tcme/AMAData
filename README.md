# AMAData
数据集说明：
1.本刺手法数据集包括教师（Teacher）和学生(Student)两个数据集

2.每类数据下面各有每个采集参加者的数据，一个人一个独立文件夹

3.每个文件夹包含六个针刺手法的原始采样数据，分别以不同的文件名保存，详细如下：

> 以tp.txt结尾：提插平补平泻
> 以tb.txt结尾：提插补法
> 以tx.txt结尾：提插泻法
> 以np.txt结尾：捻转平补平泻
> 以nb.txt结尾：捻转补法
> 以nx.txt结尾：捻转泻法

4.我们已经处理完成（机器加人工审核过的波峰波谷）的结果存在同样的文件夹中，命名如下：

> 以tp.results.txt结尾：提插平补平泻分析结果
> 以tb.results.txt结尾：提插补法分析结果
> 以tx.results.txt结尾：提插泻法分析结果
> 以np.results.txt结尾：捻转平补平泻分析结果
> 以nb.results.txt结尾：捻转补法分析结果
> 以nx.results.txt结尾：捻转泻法分析结果

5.结果中涉及识别完成的波峰和波谷点位的记录在各个result文件的前6行，以如下示例：

```
Column: 14 #选择分析的采样数据里面的哪一列
Axis: Y #选择分析的采样数据里面的这一列属于哪条轴
Fallback Frames: 0 #回滚帧数（这个暂时不用管）

Inflection point type	Point1	Point2	Point3	Point4	Point5	Point6	Point7	Point8	Point9 #这行不用管
Crests	154	267	385	497	605	710	820	938	1051 #审核过的波峰点位
Troughs	172	285	401	513	623	729	837	960	#审核过的波谷点位
#上面识别出来的点位数值是指原始采样数据的行号，第一行值是0
```
