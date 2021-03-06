## 第1章 引言
- 从数据处理、信息提取的角度来看，GIS具有一下功能
	- 数据采集与编辑：包括图形与熟悉数据的采集、编辑和分析计算。
	- 地理数据库管理：包括数据库定义、数据库的建立与维护、数据库操作、通讯等。
	- 地图制图：根据GIS的数据结构及绘图仪的类型，用户可获得矢量地图或栅格地图。
	- 空间查询与空间分析：包括拓扑空间查询、缓冲区分析、叠加分析、拓扑分析等。
	- 地形分析：包括数字高程模型建立、坡度分析、流域提取等。
- GIS不仅可以为用户输出全部要素地图，而且可以根据用户的需要分层输出各种专题地图，如行政区划图、土壤利用图、道路交通图、等高线等。另外还可以通过空间分析得到一些特殊的地理学分析用图，如坡度图、坡向图、剖面图等。
- 从接近问题的角度来看，GIS功能包含数据采集、分析、决策应用的全部过程，并能回到和解决以下五类问题：
	- 位置：在某个地方有什么。
	- 条件：复合某些条件的实体在哪里。
	- 趋势：某个地方发送某个事件及其随时间的变化过程。
	- 模式：某个地方存在的空间实体的分布模式。
	- 模拟：某个地方如果具备某种条件会发生什么。
- Python主要类库：
	- GDAL/OG，用于栅格与矢量数据的读写与处理。
	- PROJ.4，用于地图投影处理。
	- Shapely，用于数据的空间分析。
	- SpatiaLite是一个小型的空间数据库。
	- Mapnik，用于地图制图。
	- Basemap是另外一套地图制图工具。
	- 其他的，包括PyShp、GeoJSON、Descartes、GeoPandas、Folium等。