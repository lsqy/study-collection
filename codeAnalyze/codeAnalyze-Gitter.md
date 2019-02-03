# Gitter(git微信小程序）代码结构分析

## git地址

> `https://github.com/huangjianke/Gitter/`

## src

### 1、actions

> 通过redux进行异步请求的相关actions

#### 1.1、index.js

> 封装的基准action公用方法`createAction`和`createApiAction`

#### 1.2、repos.js

> 获取仓库相关的action（异步请求）

#### 1.3、trending.js

> 获取首页趋势列表的action（异步请求）

#### 1.4、user.js

> 获取用户相关的action（异步请求）

### 2、assets

#### 2.1、images

> 所需图片资源所在目录

####  2.2、ionicons

> ionicons字体图标所需的引用资源

### 3、components

> 可复用的相关组件

#### 3.1、account

> 账户相关的组件

#### 3.2、activity

> 活动相关的组件

#### 3.2、index

> 首页相关的组件

#### 3.4、repo

> 仓库相关的组件

#### 3.5、towxml

> 转换markdown的相关组件

### 4、constants

> 相关常量维护的目录

### 5、pages

> 主页面目录

#### 5.1、account

> 账户页面

#### 5.2、activity

> 活动页面

#### 5.3、index

> 首页

#### 5.4、login

> 登录页面

#### 5.5、repo

> 仓库相关页面

#### 5.6、search

> 搜索页面

### 6、reducers

> 相关的reducers的操作

### 7、service

> 封装的标准api请求

### 8、store

> redux主仓库

### 9、utils

> 封装的相关工具方法

### 10、app.js

> 框架主入口

