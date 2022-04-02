# :fa-globe: 如何优雅且合法的通过国际版reCAPTCHA验证

2022-04-02 星期六

## 前言

  为了防止机器人攻击，类似于[Mcpedl](https://mcpedl.com/ "Mcpedl")的部分下载链接，[麦块官网](https://www.minecraft.net/ "麦块官网")的购买链接还有各种大大小小的论坛和博客，都使用了该验证码。国际版reCaptcha 对于国外用户算是比较友好，但是在国内无法访问，給小白带来了“这个按钮怎么点不动啊？”的困扰。

  

  其实Google的reCAPTCHA验证是有国内版的，不过许多国外网站只考虑了国外用户的使用（~~连个简体中文都没有[~~明指Mcpedl~~]你还奢望国内版人机验证？~~），以下介绍一种比较好用的通过方法。

##   使用**Gooreplacer**重定向的方法

### 第一步 下载并安装插件

Edge：https://microsoftedge.microsoft.com/addons/detail/gooreplacer/cidbonnpjopamnhfjdgfcmjmlmehjnej

Firefox：https://addons.mozilla.org/firefox/downloads/file/3586402/gooreplacer-3.11.2-fx.xpi

{{< admonition type=tip title="⚠️提示" open=ture >}}

手机Firefox安装非精选插件需要Firefox nightly和Firefox[插件收藏集](https://addons.mozilla.org/zh-CN/firefox/collections/ "插件收藏集")的支持

{{< /admonition >}}

Chrome(不推荐，因为打不开)：https://chrome.google.com/webstore/detail/gooreplacer/jnlkjeecojckkigmchmfoigphmgkgbip

### 第二步 配置规则



    匹配模式：www.google.com/recaptcha

    匹配类型：通配符

    目标地址：recaptcha.net/recaptcha匹配模式

### 第三步 享受

这种方法支持绝大多数网站，但是并不是灵丹妙药。如果有CSP[⁽¹⁾](https://baike.baidu.com/item/CSP/13343685 "⁽百度百科详情页⁾")，可能会无法使用。
