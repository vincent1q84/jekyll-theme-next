---

title: 为什么要使用密码管理器？以及密码管理器的安全设置
date: 2020-12-22
tags: Internet

---

## 为什么要使用密码管理器？

在加州大学洛杉矶分校的网页上：

> According to Verizon’s 2017 Data Breach Investigation report, 81% of data breaches are caused by poor credential management. A password manager is the next step after DUO MFA in securing UCLA’s credentials and improving UCLA’s overall credential management. Account breaches can happen when using weak passwords or reusing old passwords/sharing passwords across accounts.-[WHY SHOULD I USE LASTPASS?](https://www.it.ucla.edu/security/services/why-should-I-use-LastPass)

泄漏密码的常见方式是使用弱密码，或者不同账号使用相同的密码。

密码管理器可以为每个网站、应用生成独立的强密码，并自动填写，使用方便。

在加州大学洛杉矶分校的网页上，[WHY USE LASTPASS](https://www.it.ucla.edu/security/services/why-should-I-use-LastPass#bootstrap-fieldgroup-accordion-item--why-use-lastpass--2-2) 一栏介绍了lastpass为什么安全。它使用最新的加密算法，网站服务器上不存储用户的主密码，也就是说 lastpass 的员工也没法知道你的主密码。

*备注*：市面上的同类密码管理器还有其它选择。比如付费的1Password和最近几年口碑较好的新晋密码管理器bitwarden（有免费版和付费版），不过bitwarden没有恢复主密码的功能（lastpass和1Password有这个功能），一旦用户自己忘了主密码，没任何办法访问自己的密码管理器。所以，使用bitwarden千万不要忘记自己的主密码。

没有恢复主密码的功能也有好处，减少了密码被盗的攻击面，盗取密码的人也没法通过恢复密码这个功能去盗取密码。

​               

有些密码管理器的免费版会限制存储密码的数量，lastpass和bitwarden的免费版不会限制存储密码的数量。

虽然现在的 android 和 iOS 自带了密码管理器，但不方便跨平台使用，也不方便添加密码笔记。lastpass、1Password和bitwarden在Windows和macOS的多个浏览器里都有扩展（比如[Chrome](https://chrome.google.com/webstore/detail/lastpass-free-password-ma/hdokiejnpimakedhajhdlcegeplioahd?hl)、[Edge](https://www.microsoft.com/en-us/p/lastpass-for-microsoft-edge/9nblggh4v7x0?activetab=pivot:overviewtab)、Safari等浏览器扩展），可以跨平台使用。（以前Edge安装过微软扩微软扩展商店等扩展后，需要重新打开Edge才能正常使用扩展，不知道现在是否有修复这个问题，Edge和Chrome内核相同，可以直接装Chrome的扩展，装过后不用重新启动Edge）

## 在 iOS 上自动填写密码

在 设置 - 密码与账户 - 自动填充密码 中，选择lastpass。（iCloud 钥匙串和 lastpass可以同时勾选。）

![autofill](https://res.cloudinary.com/djyqus4uy/image/upload/v1608639529/Blog/lastpass_ios_ees3lz.jpg)



## 为Lastpass开启两步验证

Lastpass有多种验证方式可以选。如下图，选择其中一种即可。

备注：Google Authenticator的二维码可以用authy的app添加。

![2fa](https://res.cloudinary.com/djyqus4uy/image/upload/v1608609594/Blog/lastpass_2fa_pqnl5p.jpg)

添加后点击网页下方的**update**。

如果丢了两步验证器，并且没有备份，在登陆lastpass时选择“disable” the multifactor authentication，lastpass会发一封邮件到注册邮箱里，通过邮件里的链接关闭两步验证。

## 如果忘掉lastpass主密码，如何恢复

这是可选步骤，可以开启其中的一种或几种，也可以不开启。

lastpass的博客上给出了多种方式

[链接1 指纹、Face ID等方式](https://blog.lastpass.com/2019/05/never-lose-access-lastpass-account-recovery-mobile/)

[链接2 短信](https://blog.lastpass.com/2015/10/introducing-sms-recovery-to-secure-your-account/)

备注：短信恢复需要在浏览器扩展中登陆过lastpass，此时会在本机自动保存一个随机的一次性密码，用于恢复主密码，恢复主密码时只能用曾经登陆过lastpass，生成过一次性密码的扩展。

1.指纹或者Face ID等开启方法：

在手机端登陆lastpass app后，会提示用户是否要开启指纹恢复密码的功能。如果没收到提示或者没有开启，也可以手动在settings - Secirity中开启。开启后可以在此手机的lastpass app中使用指纹恢复主密码。

![bio](https://res.cloudinary.com/djyqus4uy/image/upload/v1608610193/Blog/lastpass_bio_jef4zm.jpg)

2.短信开启方法：

在浏览器扩展里选择 open my vault，添加Recovery Phone（手机号）。



![phone](https://res.cloudinary.com/djyqus4uy/image/upload/v1608611341/Blog/lastpass_Recovery_Phone_jpg_j9axvs.jpg)

1. Sign in to LastPass via the browser extension or www.LastPass.com.登陆lastpass
2. Open your LastPass Vault. 打开你的 LastPass Vault
3. Launch the Account Settings. 启动Account Settings.
4. Scroll down to “SMS Account Recovery”. 向下滚动到“ SMS 帐户恢复”
5. Select the option to add a phone number. 选择添加电话号码的选项
6. Save your changes with the “Update” button. 用“**Update**”按钮保存更改







