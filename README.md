本站介绍：
    - 模仿别人网站的代码，编写自己的漫画网站
    - 小于576px的部分练习了一下媒体检测
    - Bootstrap5中文手册：https://www.bootstrap.cn/doc/book/2.html
        - 加上 Toast、Tooltips
        - 查看更多小工具，慢慢完善
    - √顶部导航栏：参考顶漫画，它也是用的Bootstrap5
    - √顶部轮播图：可以用swiper.js，我暂时不需要轮播图了
    - √漫画盒子：参考包子漫画 cn.baozimh.com
    - √动画盒子：天天影院+黑马前端课(遮罩)
    - √B站视频盒子：参考B站主页
    - √友情链接 + footer：参考搜片.com  soupian.pro 
    - √浮动工具栏：B站
    - comics_classify.html:参考包子漫画、顶漫画
    - √detail.html：参考了顶漫画

一些技巧：
    - img 获取src失败时，布局变乱。需要进行设置高度进行占位。为了适应响应式，这里设置为容器padding-top:130%相对定位，img绝对定位覆盖上去
    - B站API地址：https://api.bilibili.com/x/web-interface/view?bvid=BV16z421B78Z，修改BV号即可。如果是合集JSON会很长要特殊处理

待实现：
    - 研究一下导航栏的滚动怎么实现，手机端很必要
    - 可以在大盒子嵌入导航站那种的小卡片
    - 加一个滑动导航代替顶部导航？
    - 图片背景可以嵌入Bootstrap的读取图标+绝对定位
    - 用Bootstrap的form组件，例如toolbar的textarea
    - 新闻盒子参考Bootstrap的助手->延伸链接、通用类->弹性盒子->媒体对象
    - 主页是否需要设置评分的小角标
    - 主页顶部可以是左侧小轮播图 右侧几个卡片，类似B站那样
    - 跳转到details页面，可以用 手风琴/折叠 分享网站或其他内容
    - Toasts 可以每5秒显示一个新闻，主页也可以用用
    - 媒体查询时，视频盒子布局和文字大小改变一下。
    - 通过API获取视频JSON然后动态渲染标签，实现一下
    - 完善网站各个模块
    - 利用python动态更新json数据，把json当做静态数据库
    - 实现detail.html页面
    - 实现利用js从json文件提取信息，制作json文件
    - 做一下SEO优化
    - 文件结构再安排好

参考网站：
    - 天天影院：https://m.rvm2.com/ —— 页面布局
    - 包子漫画
    - 顶漫画
    - 爱壹帆

图片来源（要求无需翻墙即可访问）：
    - “B站”、茶杯狐、包子漫画
视频来源（后面详情页要设置多个源）：
    - B站、Youtube、爱壹帆、茶杯狐、金牌影院

笔记：
    :hover卡片的几种显示方式：
    - 封面图片上遮罩，标题变色
    - 封面图片放大1.25倍
    - 封面图片移入详细信息
    - 出现边框和链接下划线


# 推送到github：
    # 1. 配置 Git 账户信息
    git config --global user.name "你的用户名"
    git config --global user.email "你的邮箱"

    # 2. 进入项目目录
    cd /path/to/your/project

    # 3. 初始化本地 Git 仓库
    git init

    # 4. 添加所有文件到 Git 仓库
    git add .

    # 5. 创建初始提交
    git commit -m "Initial commit"

    # 6. 添加远程仓库
    git remote add origin https://github.com/lumengde123/mengdelu-acm.git

    # 7. 推送本地代码到远程仓库
    git branch -M main
    git push -u origin main

# 后续推送：
    # 1. 检查本地仓库状态
    git status

    # 2. 添加更改到 Git 仓库
    git add .

    # 3. 创建新的提交
    git commit -m "描述你的更改内容"

    # 4. 推送更改到远程仓库
    git push origin main

# 改变仓库名后本地需要修改
    # 1. 查看当前远程仓库 URL
    git remote -v

    # 2. 更新远程仓库 URL
    git remote set-url origin https://github.com/yourusername/new-repo-name.git

    # 3. 验证更新
    git remote -v

    # 4. 正常进行 push/pull 操作
    git pull origin main
    git push origin main


