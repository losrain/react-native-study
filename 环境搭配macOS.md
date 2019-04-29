## 环境搭配macOS
#### 安装依赖Homebrew
#### 安装依赖Node, Watchman
使用Homebrew来安装 Node 和 Watchman。在命令行中执行下列命令安装：

```
brew install node
brew install watchman
```

###### ==注意：不要使用 cnpm！cnpm 安装的模块路径比较奇怪，packager 不能正常识别==

```
npm config set registry https://registry.npm.taobao.org --global
npm config set disturl https://npm.taobao.org/dist --global
```
#### React Native 的命令行工具

```
npm install -g yarn react-native-cli
```

##### 安装 Xcode
通过 App Store 或是到Apple 开发者官网上下载
##### Xcode 的命令行工具
启动 Xcode，并在Xcode | Preferences | Locations菜单中检查一下是否装有某个版本的Command Line Tools。Xcode 的命令行工具中包含一些必须的工具，比如git等。
### 创建新项目
```
react-native init Myproject
```
##### 编译并运行 React Native 应用
```
cd Myproject
react-native run-ios
```

