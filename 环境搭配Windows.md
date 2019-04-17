## 环境搭配Windows
#### 安装依赖Node, Python2, JDK
直接使用搜索引擎搜索下载 Node 、Python2 和Java SE Development Kit (JDK)

###### ==注意：不要使用 cnpm！cnpm 安装的模块路径比较奇怪，packager 不能正常识别==

```
npm config set registry https://registry.npm.taobao.org --global
npm config set disturl https://npm.taobao.org/dist --global
```
#### React Native 的命令行工具

```
npm install -g yarn react-native-cli
```
#### Android 开发环境
##### 1. 安装 Android Studio
安装过程中确保选中了以下几项：
1. Android SDK
1. Android SDK Platform
1. Performance (Intel ® HAXM) (AMD 处理器看这里)
1. Android Virtual Device
##### 2. 配置 ANDROID_HOME 环境变量
打开控制面板 -> 系统和安全 -> 系统 -> 高级系统设置 -> 高级 -> 环境变量 -> 新建，创建一个名为ANDROID_HOME的环境变量（系统或用户变量均可），指向你的 Android SDK 所在的目录
##### 3. 把 platform-tools 目录添加到环境变量 Path 中
打开控制面板 -> 系统和安全 -> 系统 -> 高级系统设置 -> 高级 -> 环境变量，选中Path变量，然后点击编辑。点击新建然后把 platform-tools 目录路径添加进去。
##### 创建 Android 模拟器
==注意是否安装 HAXM（Intel 虚拟硬件加速驱动）==
#### 创建新项目

```
react-native init Myproject
```
##### 编译并运行 React Native 应用
```
cd Myproject
react-native run-android
```

### 热更新

```
cd Myproject
npm start
```
1. 打开Android Studio
2. import项目下的android项目
3. build完成后，启动模拟器
4. 进入模拟器选择hot loading
