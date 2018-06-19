### ninth3DHomework
这次做的游戏是一个简单的AR巡逻兵游戏，有一个巡逻兵会自动追踪角色，<br>
需要控制角色远离巡逻兵，随着时间的增加，得到的分数也会增加，同样的<br>
巡逻兵的速度也会增加，一旦被巡逻兵追到游戏结束。<br>
首先先设置好AR识别的图片，在这里我的图片是：<br>
![](https://github.com/flashowner/ninth3DHomework/blob/master/%E6%88%AA%E5%9B%BE/%E6%8D%95%E8%8E%B7.PNG)<br>
将所选择的图片添加到数据库里，然后将数据库的unitypackage包下载下来<br>
导入到项目里，同样的项目还要导入vuforia包，将原来的相机删除，将Vuforia<br>
prefabs下的ARCamera和ImageTarget拖到场景中，ARCamera是电脑的相机显示<br>
![](https://github.com/flashowner/ninth3DHomework/blob/master/%E6%88%AA%E5%9B%BE/%E6%8D%95%E8%8E%B71.PNG)
ImageTarget用来放置AR识别图片后出现的物体，在这里我使用了ImageTarget<br>
的smart Terrain，可以根据识别到的场景自动生成地形：<br>
![](https://github.com/flashowner/ninth3DHomework/blob/master/%E6%88%AA%E5%9B%BE/%E6%8D%95%E8%8E%B72.PNG)<br>
勾选后会自动生成SmartTerrain_ImageTarget，如图所示：<br>
![](https://github.com/flashowner/ninth3DHomework/blob/master/%E6%88%AA%E5%9B%BE/%E6%8D%95%E8%8E%B73.PNG)<br>
ARCamera里同样也要设置一下，世界中心为自动生成对象下的primary surface<br>
![](https://github.com/flashowner/ninth3DHomework/blob/master/%E6%88%AA%E5%9B%BE/%E6%8D%95%E8%8E%B74.PNG)<br>
然后导入下载的人物模型fighter char，自己做的巡逻兵Cube，以及人物移动的<br>
的范围wall:<br>
![](https://github.com/flashowner/ninth3DHomework/blob/master/%E6%88%AA%E5%9B%BE/%E6%8D%95%E8%8E%B75.PNG)<br>
人物的动画状态机:<br>
![](https://github.com/flashowner/ninth3DHomework/blob/master/%E6%88%AA%E5%9B%BE/%E6%8D%95%E8%8E%B76.PNG)<br>
控制人物移动的脚本：<br>
![](https://github.com/flashowner/ninth3DHomework/blob/master/%E6%88%AA%E5%9B%BE/%E6%8D%95%E8%8E%B77.PNG)<br>
巡逻兵的脚本：<br>
![](https://github.com/flashowner/ninth3DHomework/blob/master/%E6%88%AA%E5%9B%BE/%E6%8D%95%E8%8E%B78.PNG)<br>
![](https://github.com/flashowner/ninth3DHomework/blob/master/%E6%88%AA%E5%9B%BE/%E6%8D%95%E8%8E%B79.PNG)<br>
以及挂载到ARCamera下的Camera对象的GUI脚本：<br>
![](https://github.com/flashowner/ninth3DHomework/blob/master/%E6%88%AA%E5%9B%BE/%E6%8D%95%E8%8E%B710.PNG)<br>
![](https://github.com/flashowner/ninth3DHomework/blob/master/%E6%88%AA%E5%9B%BE/%E6%8D%95%E8%8E%B711.PNG)<br>
