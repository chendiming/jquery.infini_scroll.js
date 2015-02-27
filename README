当前版本：1.0.1

## What is

jquery 工具类，提供了非常轻量级、简单、实用的操作 cookie 的方法，包括读写、删除等操作。

## Live Demo
[test](http://www.baidu.com)

## Installation

1. 包含 cookie JavaScript 文件
2. 运行 $.cookie("the_cookie", "the_value");

配置选项包含：

* `trigger`      触点元素节点，仅支持一个 id 或 class 选择器
* `element`      将要开关显示的浮层节点
* `triggerType`  触发类型，click/hover，默认为click

## How to use

1. HTML结构
```
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

