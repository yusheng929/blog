---
wiki: karin-plugin-ling
title: 安装插件
---
## 安装

**以下三种方式任选其一**

* 使用编译产物{% mark build 分支 color:green %} (推荐)
{% folding child:codeblock open:false color:black 点击打开 %}

 1. 克隆源码
{% mark 务必使用 color:yellow %}以下的安装命令
{% note color:red 警告 请不要修改插件名,否则可能导致**Karin**无法识别该插件  %}
{% copy git clone --depth=1 -b build https://github.com/yusheng929/karin-plugin-ling.git ./plugins/karin-plugin-ling/ prefix:GitHub %}
如果你的Git无法访问GitHub则可以使用下方的命令
{% copy git clone --depth=1 -b build https://gitee.com/yusheng929/karin-plugin-ling.git ./plugins/karin-plugin-ling/ prefix:Gitee %}

 2. 安装依赖
请在**Karin**根目录执行
{% copy pnpm install --filter=karin-plugin-ling prefix:Karin %}
{% endfolding %}

* 使用{% mark 包管理器 color:green %} (非常推荐)
{% folding child:codeblock open:false color:black 点击打开 %}

* 在**Karin 根目录**运行
{% copy pnpm add karin-plugin-ling -w prefix:pnpm %}
{% endfolding %}

* 使用 Release {% mark build 发行版 color:green %} (不推荐)
{% folding child:codeblock open:false color:black 点击打开 %}

{%mark *不推荐该方式,后续无法通过指令或Git更新，需要重新下载 Release 更新* color:error %}

1. 打开 {% hashtag Release https://github.com/yusheng929/karin-plugin-ling/releases color:green %}
2. 找到最新版本并下载名为 {% mark build.zip color:green %} 的压缩包
3. 在 {% mark plugins/ color:green %} 目录下解压该压缩包

* 完成后相关源码应在{% mark Karin/plugins/karin-plugin-ling color:green %}
解压完成后在 **Karin根目录** 运行
{% copy pnpm install --filter=karin-plugin-ling prefix:Karin %}
{% endfolding %}
