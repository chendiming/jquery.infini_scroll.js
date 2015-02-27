当前版本：1.0.1

## What is

infini scroll jQuery 插件用来在页面滚动到屏幕底部时自动加载内容并追加 DOM 元素到页面底部，api接口友好，可能是你能找到的最简单好用的无限滚动加载插件。

## Live Demo
[点击查看在线 demo](http://csspower.fanrong33.com/csspower/javascript/infini_scroll/index.html)

## Installation

1. 包含 infini_scroll JavaScript 文件
2. 运行 $("#J_mod_article_list").infini_scroll();

配置选项包含：

* `totalPages`     总页数，默认为`0`
* `url`            获取列表url请求地址，直接返回列表的html
* `varPage`        分页变量，默认为`p`
* `triggerBottom`  距离最底部多少像素触发，默认为`100`
* `round`          默认当上拉刷新`3`次后，显示“加载更多”，防止无限制加载
* `loadingElement` 显示“正在加载更多”节点，默认`#J_loading`，一般根据自己的html结构自定义
* `loadMoreElement` 当round达到加载次数后显示的“加载更多”节点，默认`#J_load_more`
* `debug`          调试模式开关，默认`false`未开启

## How to use

1. HTML结构
````
    <ul id="J_mod_article_list" class="mod-article-list">
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
        <li>5</li>
        ...
        <li>36</li>
        <li>37</li>
        <li>38</li>
        <li>39</li>
        <li>40</li>
    </ul>
    <div id="J_loading" style="display:none;">正在加载更多</div>
    <div id="J_load_more" style="display:none;">点击加载更多</div>
```

2. JS 代码
```
    $(document).ready(function(){
        $("#J_mod_article_list").infini_scroll({
            totalPages      : 5,
            url             : "ajax_get_article_list.html",
            triggerBottom   : 1,  // test
            debug           : true
        });
    });
```

##History

记录组件的变更，请阅读[历史记录书写规范](http://csspower.sinaapp.com/rule.php#history)。

#####v1.0.1 Build 20150227

* 第一个发布版本

