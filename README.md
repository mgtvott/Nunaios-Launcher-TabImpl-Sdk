# Nunaios-Launcher-TabImpl-Sdk

# 如何引用
## 第一步

在项目的根目录的build.gradle文件中添加如下代码：

allprojects中添加
  maven {
        url "https://raw.githubusercontent.com/mgtvott/Nunaios-Launcher-TabImpl-Sdk/master"
    }

在需要使用该库的build.gradle文件的dependencies添加依赖， 代码如下


dependencies {
......省略其它依赖

implementation 'com.mgtv.nunaios.tabimpl:tabimpl:1.0.0-SNAPSHOT'

}
