<properties
   pageTitle="列出 Azure Active Directory 应用程序库中的应用程序"
   description="如何列出 Azure Active Directory 库中支持单一登录的应用程序 | Microsoft Azure"
   services="active-directory"
   documentationCenter="dev-center-name"
   authors="msmbaldwin"
   manager="mbaldwin"
   editor=""/>

<tags
   ms.service="active-directory"
   ms.date="02/19/2016"
   wacn.date=""/>


# 列出 Azure Active Directory 应用程序库中的应用程序

若要列出 [Azure AD 库](/marketplace/active-directory/all/)中支持使用 Azure Active Directory 进行单一登录的应用程序，该应用程序首先需要实现下列集成模式之一：

* **OpenID Connect** - 与 Azure AD 直接集成，使用 OpenID Connect 进行身份验证，并使用 Azure AD 许可 API 进行配置。如果你刚刚开始集成并且你的应用程序不支持 SAML，则这是建议的模式。

* **SAML** – 你的应用程序已经能够使用 SAML 协议配置第三方标识提供者。

下面显示了每种模式的列出要求。

##OpenID Connect 集成

若要将你的应用程序与 Azure AD 集成，请遵循[开发人员说明](active-directory-authentication-scenarios.md)。然后回答以下问题并发送到 waadpartners@microsoft.com。

* 提供应用程序测试租户或帐户的凭据，使 Azure AD 团队可以测试集成。  

* 为 Azure AD 团队提供有关如何使用 [Azure AD 许可框架](https://azure.microsoft.com/documentation/articles/active-directory-integrating-applications/#overview-of-the-consent-framework)登录并将 Azure AD 实例连接到应用程序的说明。

* 为 Azure AD 团队提供在应用程序上测试单一登录所需的其他说明。

* 提供以下信息：

> 公司名称：
> 
> 公司网站：
> 
> 应用程序名称：
> 
> 应用程序说明（限制为 256 个字符）：
> 
> 应用程序网站（参考性）：
> 
> 应用程序技术支持网站或联系信息：
> 
> 应用程序的客户端 ID，在 https://manage.windowsazure.com 上的应用程序详细信息中显示：
> 
> 客户注册和/或购买应用程序时所用的应用程序注册 URL：
> 
> 选择应用程序所要列入到的最多三个类别（有关可用类别，请参阅“Azure Active Directory 应用商店”）：
> 
> 附加应用程序小图标（PNG 文件，45 x 45 像素，实色背景）：
> 
> 附加应用程序大图标（PNG 文件，215 x 215 像素，实色背景）：
> 
> 附加应用程序徽标（PNG 文件，150 x 122 像素，透明背景色）：

##SAML 集成

如果[使用这些说明添加自定义应用程序](active-directory-saas-custom-apps.md)，支持 SAML 2.0 的任何应用程序都可直接与 Azure AD 租户集成。应用程序经测试可与 Azure AD 集成后，请将以下信息发送到 <waadpartners@microsoft.com>。

* 提供应用程序测试租户或帐户的凭据，使 Azure AD 团队可以测试集成。  

* 按[此处](active-directory-saas-custom-apps.md)所述提供应用程序的 SAML 登录 URL、颁发者 URL（实体 ID）和回复 URL（断言使用者服务）的值。如果你一般情况下在 SAML 元数据文件中提供了这些值，请随附该文件。

* 提供有关如何在使用 SAML 2.0 的应用程序中配置 Azure AD 作为标识提供者的简短描述。如果应用程序支持通过自助服务管理门户将 Azure AD 配置为标识提供者，请确保上面提供的凭据可用于进行此项设置。

* 提供以下信息：

> 公司名称：
> 
> 公司网站：
> 
> 应用程序名称：
> 
> 应用程序说明（限制为 256 个字符）：
> 
> 应用程序网站（参考性）：
> 
> 应用程序技术支持网站或联系信息：
> 
> 客户注册和/或购买应用程序时所用的应用程序注册 URL：
> 
> 选择应用程序所要列入到的最多三个类别（有关可用类别，请参阅 [Azure Active Directory 应用商店](https://azure.microsoft.com/marketplace/active-directory/)）：
> 
> 附加应用程序小图标（PNG 文件，45 x 45 像素，实色背景）：
>
> 附加应用程序大图标（PNG 文件，215 x 215 像素，实色背景）：
>
> 附加应用程序徽标（PNG 文件，150 x 122 像素，透明背景色）：

<!---HONumber=Mooncake_0411_2016-->