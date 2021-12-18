# GNSS浮标数据共享

### 共享动机

GNSS浮标一种古老而又新颖的测量设备，在海洋具有广泛的应用场景。当前我国海洋调查数据共享普遍较弱，而GNSS浮标的研究由于更加小众，网上很难找到此类数据。为了促进国内学者进行相关研究工作，决定公开GNSS浮标数据。

### 数据表

| 时间 | 地点 | 基站 |航迹| 用途 |
| --- | --- | --- | --- | --- |
| 20140707-0709 | 青岛千里岩 | Y |Y| 卫星高度计定标 |
| 20140915-0919 | 青岛千里岩 | Y |N| 卫星高度计定标 |
| 20141015-1015 | 青岛田横岛 | Y |N|卫星高度计定标 |
| 20150410-0410 | 青岛田横岛 | Y |N| 卫星高度计定标 |
| 20150502-0502 | 珠海担杆岛 | Y |Y| 卫星高度计定标 |
| 20150629-0701 | 青岛千里岩 | Y |N| 卫星高度计定标 |
| 20190331-0401 | 青岛小麦岛 | Y |Y| 机载高度计定标 |
| 20190714-0715 | 威海成山头 | Y |Y| 卫星高度计定标 |
| 20190826-0827 | 威海成山头 | Y |Y| 卫星高度计定标 |
| 20210520-0524 | 青岛小麦岛 | N |Y| 低成本浮标测试 |

### 数据下载

https://zenodo.org/record/5774652


### 数据描述

数据格式主要为GNSS通用RINEX格式。少数试验数据为硬件厂家格式，使用者需要使用相关软件进行格式转换。

### 数据解算软件

很多软件可以用于解算动态的浮标数据，比如：
- [GAMIT](http://geoweb.mit.edu/gg/)
- [Bernese GNSS](http://www.bernese.unibe.ch/)
- [RTKLIB](http://www.rtklib.com/)
- [PRIDE PPP-AR](http://pride.whu.edu.cn/indexone.shtml)
- [CSRS-PPP](https://webapp.geod.nrcan.gc.ca/geod/tools-outils/ppp.php)

我们发现RtkLib容易上手，PPPpride对廉价芯片数据的处理更加优秀，CSRS-PPP更加智能化。GAMIT有点老，但是很经典，Bernese功能强大，是收费软件。此外还有一些其他的商业或者免费软件可以分析GNSS数据，无法一一列举。

### 浮标应用场景

本次共享的GNSS浮标数据主要是卫星高度计定标项目所采集，因此也主要用于了海面高度和海浪测量。GNSS浮标可以准确的获得地心坐标系下的三维海面起伏，数据频率通常使用1Hz，可以有效的提取潮汐信息和波浪信息。
- 卫星高度计定标
- 机载高度计定标
- 远海潮汐测量
- 波浪全要素测量
- 大地水准面评估

它还有很多应用没有挖掘，更多信息见：[小型低成本GNSS浮标研发及初步结果](https://mp.weixin.qq.com/s?__biz=Mzg3MDU0MjYwMw==&mid=2247484478&idx=1&sn=0b724d0a3e9818c1c0e69e5e45bdbb6e&chksm=ce8d785af9faf14cccef5a21da24b1c0bc1aacb3c2b2bb7a083a21106c1d73b39cac74647d57&token=1728212089&lang=zh_CN#rd)

### 引用

数据引用格式：
```
@dataset{lei_yang_2021_5774652,
  author       = {Lei Yang},
  title        = {GNSS buoy data},
  month        = dec,
  year         = 2021,
  publisher    = {Zenodo},
  doi          = {10.5281/zenodo.5774652},
  url          = {https://doi.org/10.5281/zenodo.5774652}
}
```

如果数据对您的研究有用，也可以考虑引用如下论文：

[1]LIN Z, LEI Y, YONGSHENG X, 等. Retrieving wave parameters with PPP mode from GNSS buoy measurements[J]. IEEE Geoscience and Remote Sensing Letters, 2020, Early Access. DOI:10.1109/LGRS.2020.3041846.

[2]LEI Y, XINGHUA Z, P. M S, 等. First Calibration Results of Jason-2 and Saral/AltiKa Satellite Altimeters from the Qianliyan Permanent Facilities[J]. Advances in Space Research, 2017, 59(12): 2831–2842. DOI:https://doi.org/10.1016/j.asr.2017.02.044.

[3]YANG L, XU Y, ZHOU X, 等. Calibration of an Airborne Interferometric Radar Altimeter over the Qingdao Coast Sea, China[J]. Remote Sensing, 2020, 12(10): 1651. DOI:10.3390/rs12101651.

[4]杨磊, 周兴华, 王朝阳, 等. 基于GNSS浮标和验潮资料的HY-2A卫星雷达高度计绝对定标[J]. 海洋学报, 2017, 39(1): 111–120.


