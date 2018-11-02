---
title:  Woocommerce ERC20 Payment Gateway 插件
date: 2018-11-01 11:47:47
tags:
---

作为世界上使用人数最多的 CMS （内容管理系统），WordPress 拥有大量的拥趸，而 WooCommerce 作为 WordPres 中使用人数最多的商城插件，自然很适合帮助创业者快速建立起一个完善的商城工具。

![](https://postimg.aliavv.com/newmbp/pu2lg.png)

**WooCommerce ERC20 Payment Gateway** 是 Inkerk Blockchain Inc. 开发的一款用于 WooCommerce 的支付网关插件，能够为基于 WordPress 和 WooCommerce 的在线商城引入 ERC20 支付功能。

### 插件功能

1. 原生的 ERC20 Token 的支持
2. 交易 tx 记录在订单信息中
3. 支持自定义 Token 名称（由 Woocommerce Customize ERC20 Currency 插件完成)

### 支付说明

**插件当前版本仅在订单备注中记录了 tx ，没有进行订单状态的自动变更，因此，需要管理员自行处理订单。后续会随着插件迭代逐步考虑实现自动更新订单状态。**

用户支付完成后，在订单的备注中会记录交易的 tx ，备查。

![](https://postimg.aliavv.com/newmbp/esajf.jpg)

### 安装插件

访问 WordPress 后台，在添加插件页面搜索 「**WooCommerce ERC20 Payment Gateway**」，在搜索结果中找到插件并安装即可。

![](https://postimg.aliavv.com/newmbp/2wru5.jpg)

### 配置插件

**安装并启用插件后**，需要对插件进行一定的配置后才可以正常使用。

打开 「**WooCommerce**」—「**设置**」—「**付款**」

![](https://postimg.aliavv.com/newmbp/dmxxc.jpg)

在这里你可以看到多种不同的支付方式。**关闭其他的支付方式**，并**启用*使用 ERC 20 Token 支付*** 支付方式。

勾选为启用后，点击下方的保存更改，启用 ERC 20 Token 支付。

启用成功后，点击支付方式后的「管理」按钮，进入到网关设置界面。

#### 基础配置

![](https://postimg.aliavv.com/newmbp/q9zt8.jpg)

首先是配置支付网关的信息。设置支付方式的标题，引导客户使用对应的 Token 支付，建议设置为「使用 XXX 支付」，语义明确。三者位置示意图如下：

![](https://postimg.aliavv.com/newmbp/7m735.jpg)

在完成了支付方式的设置后，就需要配置 Metamask 支付参数了。

#### 支付参数

![](https://postimg.aliavv.com/newmbp/0jvum.jpg)

支付参数一共有4项，分别是

1. **钱包地址**：钱包地址需要填入收款人的地址。也就是商店主人的钱包地址。
2. **合约 ABI**：合约 ABI 用于发起转账，你可以在 etherscan.io 上的合约页面中找到它。
3. **合约地址**：合约的地址用于发起转账，你可以在 etherscan.io 找到它。
4.  **Gas 提醒**：Gas 提醒将会展示在支付界面，用于提醒用户支付较高的 gas ，从而可以提升交易完成的速度。

### 帮助内容

#### 如何找到 ABI ？

打开 Etherscan ，找到你自己的合约，找到 Code 一栏。

![](https://postimg.aliavv.com/newmbp/jhhpc.jpg)

向下拖动后，可以找到合约的ABI，点击这里的 **Copy** 按钮，然后粘贴到插件设置界面即可。

![](https://postimg.aliavv.com/newmbp/519dv.jpg)

### 相关链接

WordPress 官方插件市场：https://wordpress.org/plugins/woo-erc20-payment-gateway/

Github ：https://github.com/inKerk/woocommerce-erc20-payment-gateway