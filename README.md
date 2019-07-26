## 项目说明

- [WeTypecho][1]作为小程序版typecho十分有名，但苦于handsome主题与其不兼容（图片加载不出来）。在网上得到[xiaoningboke][2]大佬的启发后，本人进行进一步修改，最终得到此版本在此向各位大佬致谢。

 **说明**
 - **小程序内web-view组件需要业务域名，因此暂不支持直接点开链接**
 - **暂不支持小程序内点开图片**


## 项目地址

 - [https://github.com/oduang/wetypecho-for-handsome/][3]


## 修改内容

 1. 修复文章头图不显示的问题
 2. 修复轮播文字头图不显示的问题
 3. 修复排行文章头图不显示的问题
 4. 修复相关阅读文章头图不显示的问题
 5. 修复搜索列表文章头图不显示的问题
 6. 关于页添加默认图片
 7. 更新小程序授权登录页面代码
 8. 强制修改首页显示最近发布
 9. 调整文章整体上下之间的空隙
 10. 优化部分css样式
 11. 关于页禁止他人评论，仅仅用户开发者可以评论（须配置openID，适用于handsome的时光机）
 12. 添加小程序更新代码

## 小程序案例

![xcx.jpg][4]

## 使用方法
 - **通用修改**

   - 原版修改说明:
   - [https://2012.pro/index.php/20180811/cid=77.html][5]

 - **自定义修改（修改为自己的地址,前面数字为行数）**
 
 1. **page/index/index.js**
     ```
     42: datas[i].image = "../../resources/logo.jpg"
     94：datas[i].image = "../../resources/logo.jpg"
     ```
 2. **page/cat/cat.js**
    ```
    108： datas[i].image = "../../resources/logo.jpg"
    ```
 3. **page/about/about.js(貌似不支持本地加载)**
    ```
    176: item.authorImg = 'https://oduang.com/logo.jpg';
    ```
 4. **page/detail/detail.js(貌似不支持本地加载)**
    ```
    117： datas[i].image = "../../resources/logo.jpg"`
    197： item.authorImg = 'https://oduang.com/logo.jpg';
    ```
 5. **page/list/list.js**
    ```
    44: datas[i].image = "../../resources/logo.jpg"
    ```

## 感谢

本项目深度感谢以下大佬
- https://github.com/MingliangLu/WeTypecho
- https://github.com/xiaoningboke/WeTypecho
- https://github.com/yyzheng1729/loginDemo
- https://blog.csdn.net/qq_43327305/article/details/85919586


  [1]: https://2012.pro/index.php/20180806/cid=37.html
  [2]: https://www.sunxiaoning.com/live/792.html
  [3]: https://github.com/oduang/weytpecho-for-handsome/
  [4]: https://oduang.com/usr/uploads/2019/07/147765595.jpg
  [5]: https://2012.pro/index.php/20180811/cid=77.html
