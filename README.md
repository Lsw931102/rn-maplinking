# rn-maplinking主要功能
react native 唤醒第三方地图app实现富标注、线路规划、导航
目前支持 android：高德地图、百度地图、腾讯地图  ios：高德地图、百度地图、腾讯地图、苹果地图
 
# 使用
注意：
      使用时若发现调起页面不正确，请自行去各个地图的官网查看官方文档是否有更新，一下附上官方文档地址
      高德地图：https://lbs.amap.com/api/amap-mobile/summary
      百度地图：http://lbsyun.baidu.com/index.php?title=uri/api/android
      腾讯地图：https://lbs.qq.com/uri_v1/index.html
  
如何使用：
      在需要调用的组件中import引入MapLinking，然后调用需要用到的方法（markLocation添加富标注、planRoute路径规划、navigate导航），按照需要的参数依次传入相应的参数。
      eg. MapLinking.planRoute(
             {
              lat: fromLat,
              lng: fromLng,
              type: "gcj02",
              title: fromAddr
            },
            {
              lat: destLat,
              lng: destLng,
              type: "gcj02",
              title: destAddr
            },
            "ride"
          )

使用前请先阅读各个地图调起的前提，去注册相应的信息
