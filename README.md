# Google-Browser
谷歌浏览器高版本设置跨域终极解决方案  

## 三步解决

### 安装和卸载
**卸载**

> window 左下角 开始->设置->应用，找到安装过的google浏览器
<div align="left">
  <img src="https://user-images.githubusercontent.com/21699695/146565378-da7c7610-1569-40e4-a91d-f8705f6c5bd6.png" alt="Editor" width="300">
</div>  

**安装**  
[Google浏览器历史版本列表1](https://www.chromedownloads.net/chrome64win/)  
[Google浏览器历史版本列表2](https://filehippo.com/download_google-chrome/history/)  
> 两个最全列表，推荐第一个链接下载指定版本，哪个能访问下载哪一个。  

**跨域的话建议使用低版本的，我下载的是87版本的**

### 禁用浏览器自动更新
**最暴力方便的方法**  
> 1.C盘中把GoogleUpdate.exe文件改个名，这个是Chrome默认的安装位置（应该）  

<div align="left">
  <img src="https://user-images.githubusercontent.com/21699695/146568603-d7c53216-3ad8-4305-aac2-084df4d723b3.png" alt="Editor" width="200">
</div> 

>2. 修改名称，GoogleUpdate.exe加个字符即可  
<div align="left">
  <img src="https://user-images.githubusercontent.com/21699695/146569451-52cf0345-2c83-4318-a639-d148fbf072b8.png" alt="Editor" width="300">
</div>  

>3.假如点关于还是会更新到最新版本，这有一个补偿方法  
* 在来Update文件夹上右键，在属性里的安全页签里点击编辑，设置system完全控制权设置为拒绝，administrator权限也是它赋予的。
* System是最高权限，设置完了之后google就没有权限动这个文件了
* 如图就是限制update文件夹权限
<div align="left">
  <img src="https://user-images.githubusercontent.com/21699695/146571158-1af191a8-93d7-4714-ad02-c63dc436dca5.png" alt="Editor" width="300">
</div>  

### 设置跨域
> 复制一个google浏览器快捷键 右键‘属性’，‘快捷方式’，‘目标’ 路径最后边按一下空格  

```js
--args --disable-web-security --user-data-dir=D:\HaoroomsChromeUserData
```
**91版本之前**  
> chrome://flags
地址栏输入**chrome://flags**并回车
搜索栏中输入**SameSite by default cookies**搜索,会有两项设置
改为**Disabled**后重启浏览器即可  

**91版本之后, 94已移除**  
```js
--disable-features=SameSiteByDefaultCookies,CookiesWithoutSameSiteMustBeSecure
```
<div align="left">
  <img src="https://user-images.githubusercontent.com/21699695/146574166-2099853c-a11f-4c20-9774-844ac2380db6.png" alt="Editor" width="300">
</div>

**我使用的是86版本的，根据你的版本来搜索解决方案**  

**强烈推荐福利！！！每天免费领取饿了么，美团外卖红包（买菜，点美食都可以）**

<div align="left">
  <img src="https://user-images.githubusercontent.com/21699695/221159459-81384c4b-67a0-4616-b885-515965989fa4.png" alt="Editor" width="600">
</div>

**互相学习交流**

<div align="left">
  <img src="https://user-images.githubusercontent.com/21699695/123603292-4f911180-d82c-11eb-809b-9c9f6232ba04.png" alt="Editor" width="200">
</div>
