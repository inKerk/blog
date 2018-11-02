---
title: Woocommerce Customize ERC20 Currency 插件
date: 2018-11-01 11:53:49
tags:
---



在开发 Woocommerce 的 ERC20 Token 支付插件时，我们发现了一个问题，现有的 ERC20 支付插件往往是基于现有的货币体系来实现的，也就是从一开始，其锚定的货币便是某一种法币，比如，人民币、美元、商品的价格计算都是基于法币进行的，这样会导致插件需要考虑不同货币之间的换算，以及在数字货币之间的换算问题，稍有不慎，就设置错误了。

我们考虑，开发一款原生支持 ERC20 Token 的插件，来满足支付的需求，那么就要求 Woocommerce 能够以 ERC20 Token 来作为商城的支付货币，但是，Woocommerce 默认的货币系统中并不包含 ERC20  Token。

因此，为了方便用户在自己的商城中加入 ERC20 Token ，我们开发出了 「Woocommerce Customize ERC20 Currency」 插件。

**Woocommerce Customize ERC20 Currency** 插件能够为 WooCommerce 添加自定义货币的功能，推荐和 Woocommerce ERC20 Payment Gateway 插件联合使用。



## Woocommerce Customize ERC20 Currency 的安装

**Woocommerce Customize ERC20 Currency **目前已经上架 WordPress 官方商城，因此，你可以直接在 WordPres 后台安装相关插件。

> 安装 Woocommerce Customize ERC20 Currency 前请确保你已经安装并启用了 WooCommerce。

访问 WordPress 后台的插件安装界面,在右上角搜索框内输入「**Woocommerce Customize ERC20 Currency**」，然后点击搜索，在搜索结果中即可看到插件。

![](https://postimg.aliavv.com/newmbp/e3yp9.jpg)

点击现在安装，即可安装插件。

## 插件配置

**安装并启用插件**后，就可以配置插件了。

打开后台侧边栏「 Settings」-「WooCommerce ERC20 货币自定义」页面，可以自定义货币的名称和符号。

![](https://postimg.aliavv.com/newmbp/x0w09.jpg)

在设置界面，你可以设置自定义货币的名称，以及其对应的符号。

![](https://postimg.aliavv.com/newmbp/uqun9.jpg)

货币名称将会显示在列表中，用于选择不同的货币，货币符号则可以根据设置，显示在价格的前后，其作用类似于人民币的`¥` 和美元的 `$`。

## 修改货币

设置完自定义的货币后，你就可以设置 WooCommerce 的支付货币了。

打开后台侧边栏 「WooCommerce」—「设置」，将界面拖动到底部，可以看到币种选择。

![](https://postimg.aliavv.com/newmbp/vvebf.jpg)

在币种选择中，选择你自己的货币。

![](https://postimg.aliavv.com/newmbp/zxhyj.jpg)

并设置货币符号的显示的位置，并保存。

![](https://postimg.aliavv.com/newmbp/nh9v8.jpg)

这样，就完成了 WooCommerce 使用自定义的货币的功能了。

前台展示效果如下：

![](https://postimg.aliavv.com/newmbp/sqsi3.jpg)



## 相关链接

项目 Github 地址：https://github.com/inKerk/woocommerce-custom-erc20-currencies

WordPress 官方市场地址：https://wordpress.org/plugins/woo-custom-erc20/