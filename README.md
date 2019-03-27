# Nunaios-Launcher-TabImpl-Sdk

# 如何引用
## 第一步

在项目的根目录的build.gradle文件中添加如下代码：



allprojects中添加

```
  maven {
        url "https://raw.githubusercontent.com/mgtvott/Nunaios-Launcher-TabImpl-Sdk/master"
       }
```  
    
    
在需要使用该库的build.gradle文件的dependencies添加依赖， 代码如下


```
dependencies {
  #......省略其它依赖

   compile ('com.mgtv.nunaios.tabimpl:tabimpl:1.0.1-SNAPSHOT'){ changing = true }

}
```


在build.gradle 最后加上如下内容

```
configurations.all {
    // 动态版本(版本号会变)
    resolutionStrategy.cacheDynamicVersionsFor 1, 'minutes'
    // 变化模块(版本号永远不变,但是内容发生变化)
    resolutionStrategy.cacheChangingModulesFor 0, 'minutes'
}
```


