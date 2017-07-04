# \<head>

[![CC0](https://img.shields.io/badge/license-CC0-green.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![Contributors](https://img.shields.io/github/contributors/joshbuchea/head.svg)](https://github.com/joshbuchea/HEAD/graphs/contributors)
[![Amazon Referral](https://img.shields.io/badge/referral-amazon-yellow.svg)](https://amazon.com/?tag=buchea-20)

A list of everything that could go in the `<head>` of your document

## Table of Contents

- [Recommended Minimum](#recommended-minimum)
- [Elements](#elements)
- [Meta](#meta)
- [Link](#link)
  - [Favicons](#favicons)
- [Social](#social)
  - [Facebook Open Graph](#facebook-open-graph)
  - [Facebook Instant Articles](#facebook-instant-articles)
  - [Twitter Cards](#twitter-cards)
  - [Google+ / Schema.org](#google--schemaorg)
  - [OEmbed](#oembed)
- [Browsers / Platforms](#browsers--platforms)
  - [Apple iOS](#apple-ios)
  - [Apple Safari](#apple-safari)
  - [Google Android](#google-android)
  - [Google Chrome](#google-chrome)
  - [Microsoft Internet Explorer](#microsoft-internet-explorer)
- [Browsers (Chinese)](#browsers-chinese)
  - [360 Browser](#360-browser)
  - [QQ Mobile Browser](#qq-mobile-browser)
  - [UC Mobile Browser](#uc-mobile-browser)
- [App Links](#app-links)
- [Notes](#notes)
  - [Performance](#performance)
- [Other Resources](#other-resources)
- [Related Projects](#related-projects)
- [Other Formats](#other-formats)
- [Translations](#translations)
- [Contributing](#contributing)
- [Contributors](#contributors)
- [Author](#author)
- [License](#license)

## Recommended Minimum最低要求

Below are the essential tags for basic, minimalist websites:

下面是至关重要的基础性标签，极简主义网站

```html
<meta charset="utf-8">
<meta http-equiv="x-ua-compatible" content="ie=edge">
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
<!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
<!-- 以上3个meta标签 *必须* 放到head里的最前面;其他head里的内容必须放倒这些标签的*后面* -->
<title>Page Title</title>
```

## Elements元素

``` html
<!-- Document Title -->
<!-- 文档标题 -->
<title>Page Title</title>

<!-- Base URL to use for all relative URLs contained within the document -->
<!-- base URL用于document内所有相对URL, -->
<base href="https://example.com/page.html">

<!-- External CSS -->
<!-- 外部css -->
<link rel="stylesheet" href="styles.css">

<!-- In-document CSS -->
<!-- 内部文档 css -->
<style>
  /* ... */
</style>

<!-- JavaScript -->
<script src="script.js"></script>
<noscript>
  <!--no JS alternative-->
  <!-- 没有js的替代区域 -->
</noscript>
```

## Meta

``` html
<meta charset="utf-8"> 
<!-- set character encoding for the document -->
<!-- 设置文档字符编码 -->
<meta http-equiv="x-ua-compatible" content="ie=edge">
<meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
<!-- The above 3 meta tags *must* come first in the head; any other head content must come *after* these tags -->
<!-- 下面3个meta标签*必须*放倒head里的最前面；任何其他head内容必须放到这些标签的*后面* -->

<!-- Allows control over where resources are loaded from -->
<!-- 限制所有的外部加载的资源 -->
<meta http-equiv="Content-Security-Policy" content="default-src 'self'">
<!-- Place as early in the document as possible -->
<!-- 尽可能早的在文档中放置 -->
<!-- Only applies to content below this tag -->
<!-- 只适用此标签下面的内容 -->

<!-- Name of web application (only should be used if the website is used as an app) -->
<!-- web应用的名字（只在网站被用于应用的时候使用） -->
<meta name="application-name" content="Application Name">

<!-- Short description of the page (limit to 150 characters) -->
<!-- 页面的短描述（限制在150个字符） -->
<!-- In *some* situations this description is used as a part of the snippet shown in the search results. -->
<!-- 在*某些*情况下，此描述用作搜索结果中显示片段的一部分 -->
<meta name="description" content="A description of the page">

<!-- Control the behavior of search engine crawling and indexing -->
<!-- 控制搜索引擎爬行和索引的行为 -->
<meta name="robots" content="index,follow">
<!-- All Search Engines 所有的搜索引擎 -->
<meta name="googlebot" content="index,follow">
<!-- Google Specific 只针对google -->

<!-- Tells Google not to show the sitelinks search box -->
<!-- 告诉google不要显示网站链接的搜索框里 -->

<meta name="google" content="nositelinkssearchbox">

<!-- Tells Google not to provide a translation for this page -->
<!-- 告诉google不要为这个页面提供翻译 -->
<meta name="google" content="notranslate">

<!-- Verify ownership for Google Search Console -->
<!-- 验证google搜索控制台的所有权 -->
<meta name="google-site-verification" content="verification_token">

<!-- Verify ownership for Yandex Webmasters -->
<!-- 验证Yandex网站的所有权 -->
<meta name="yandex-verification" content="verification_token">

<!-- Verify ownership for Bing Webmaster Center -->
<!-- 验证Bing网站中心的所有权 -->
<meta name="msvalidate.01" content="verification_token">

<!-- Verify ownership for Alexa Console -->
<!-- 验证Alexa控制台的所有权 -->
<meta name="alexaVerifyID" content="verification_token">

<!-- Verify ownership for Pinterest Console-->
<!-- 验证Pinterest控制台的所有权 -->
<meta name="p:domain_verify" content="code from pinterest">

<!-- Verify ownership for Norton Safe Web -->
<!-- 沿着个Norton安全网站的所有权 -->
<meta name="norton-safeweb-site-verification" content="norton code">

<!-- Used to name software used to build the website (i.e. - WordPress, Dreamweaver) -->
<!-- 用于命名构建网站的软件（例如：-wordpress,dreamweaver） -->
<meta name="generator" content="program">

<!-- Short description of your site's subject -->
<!-- 你站点主题的短描述 -->
<meta name="subject" content="your website's subject">

<!-- Gives a general age rating based on sites content -->
<!-- 根据网站内容给出General的年龄等级 -->
<meta name="rating" content="General">

<!-- Allows control over how referrer information is passed -->
<!-- 允许控制referrer信息如何被通过 -->
<meta name="referrer" content="no-referrer">

<!-- Disable automatic detection and formatting of possible phone numbers -->
<!-- 禁用自动检测和格式化可能的电话号码 -->
<meta name="format-detection" content="telephone=no">

<!-- Completely opt out of DNS prefetching by setting to 'off' -->
<meta http-equiv="x-dns-prefetch-control" content="off">

<!-- Stores cookie on the client web browser for client identification -->
<!-- 在客户端web浏览器上存储cookie，用于提供客户端识别 -->
<meta http-equiv="set-cookie" content="name=value; expires=date; path=url">

<!-- Specifies the page to appear in a specific frame -->
<!-- 指定出现在特殊frame中的页 -->
<meta http-equiv="Window-Target" content="_value">

<!-- Geo tags -->
<!-- Geo标签 -->
<meta name="ICBM" content="latitude, longitude">
<meta name="geo.position" content="latitude;longitude">
<meta name="geo.region" content="country[-state]"><!-- Country code (ISO 3166-1): mandatory, state code (ISO 3166-2): optional; eg. content="US" / content="US-NY" -->
<meta name="geo.placename" content="city/town"><!-- eg. content="New York City" -->
```

- [Meta tags that Google understands](https://support.google.com/webmasters/answer/79812?hl=en)
- [WHATWG Wiki: MetaExtensions](https://wiki.whatwg.org/wiki/MetaExtensions)
- [ICBM on Wikipedia](https://en.wikipedia.org/wiki/ICBM_address#Modern_use)
- [Geotagging on Wikipedia](https://en.wikipedia.org/wiki/Geotagging#HTML_pages)


## Link

``` html
<!-- Points to a CSS stylesheet -->
<!-- 指向css样式 -->
<link rel="stylesheet" href="https://example.com/styles.css">

<!-- Helps prevent duplicate content issues -->
<!-- 帮助放置重复的内容问答 -->
<link rel="canonical" href="https://example.com/2010/06/9-things-to-do-before-entering-social-media.html">

<!-- Used to be included before the icon link, but is deprecated and no longer is used -->
<!-- 用于被包括在icon链接之前，但已经被废弃不再使用 -->
<link rel="shortlink" href="https://example.com/?p=42">

<!-- Links to an AMP HTML version of the current document -->
<!-- 链接到当前文档的AMP HTML版本 -->
<link rel="amphtml" href="https://example.com/path/to/amp-version.html">

<!-- Links to a JSON file that specifies "installation" credentials for web applications -->
<!-- 链接到JSON文件，指定web应用的"安装"凭据 -->
<link rel="manifest" href="manifest.json">

<!-- Links to the author of the document -->
<!-- 链接到作者文档 -->
<link rel="author" href="humans.txt">

<!-- Refers to a copyright statement that applies to the links context -->
<!-- 制适用于链接背景的版权声明 -->
<link rel="license" href="copyright.html">

<!-- Gives a reference to a location in your document that may be in another language -->
<!-- 给一个你的文档另一种语言版本的参考地址 -->
<link rel="alternate" href="https://es.example.com/" hreflang="es">

<!-- Gives information about an author or another person -->
<!-- 提供关于作者或者其他人的信息 -->
<link rel="me" href="https://google.com/profiles/thenextweb" type="text/html">
<link rel="me" href="mailto:name@example.com">
<link rel="me" href="sms:+15035550125">

<!-- Links to a document that describes a collection of records, documents, or other materials of historical interest. -->
<!-- 链接一个文档，用于描述历史记录，文档或是其他历史资料的集合 -->
<link rel="archives" href="https://example.com/archives/">

<!-- Links to top level resource in an hierarchical structure -->
<!-- 在层次结构中链接到顶级资源 -->
<link rel="index" href="https://example.com/">

<!-- Gives a self reference - useful when the document has multiple possible references -->
<!-- 当文档具有多种可能的引用时，提供一个自引用 -->
<link rel="self" type="application/atom+xml" href="https://example.com/atomFeed.php?page=3">

<!-- The first, next, previous, and last documents in a series of documents, respectively -->
<!-- 分别链接到一系列文档中的第一个，下一个，前一个，最后一个 -->
<link rel="first" href="https://example.com/atomFeed.php">
<link rel="next" href="https://example.com/atomFeed.php?page=4">
<link rel="prev" href="https://example.com/atomFeed.php?page=2">
<link rel="last" href="https://example.com/atomFeed.php?page=147">

<!-- Used when using a 3rd party service to maintain a blog -->
<!-- 在使用第三方服务维护博客时使用 -->
<link rel="EditURI" href="https://example.com/xmlrpc.php?rsd" type="application/rsd+xml" title="RSD">

<!-- Forms an automated comment when another WordPress blog links to your WordPress blog or post -->
<!-- 当其他的WordPress博客链接到你的WordPress博客或者文章时，形成一个自动评论 -->
<link rel="pingback" href="https://example.com/xmlrpc.php">

<!-- Notifies a url when you link to it on your site -->
<!-- 当你的站点链接到URL时通知它 -->
<link rel="webmention" href="https://example.com/webmention">

<!-- Loads in an external HTML file into the current HTML file -->
<!-- 加载一个外部HTML文件到当前HTML文件中 -->
<link rel="import" href="/path/to/component.html">

<!-- Open Search -->
<!-- 开放搜索 -->
<link rel="search" href="/open-search.xml" type="application/opensearchdescription+xml" title="Search Title">

<!-- Feeds -->
<link rel="alternate" href="https://feeds.feedburner.com/example" type="application/rss+xml" title="RSS">
<link rel="alternate" href="https://example.com/feed.atom" type="application/atom+xml" title="Atom 0.3">

<!-- Prefetching, preloading, prebrowsing -->
<!-- 预提取，预加载，预浏览 -->
<link rel="dns-prefetch" href="//example.com/">
<link rel="preconnect" href="https://www.example.com/">
<link rel="prefetch" href="https://www.example.com/">
<link rel="prerender" href="https://example.com/">
<link rel="preload" href="image.png" as="image">
<!-- More info: https://css-tricks.com/prefetching-preloading-prebrowsing/ -->
```

### Favicons

``` html
<!-- For IE 10 and below -->
<!-- Place favicon.ico in the root directory - no tag necessary -->

<!-- For IE 11, Chrome, Firefox, Safari, Opera -->
<link rel="icon" type="image/png" sizes="16x16" href="/path/to/favicon-16x16.png">
<link rel="icon" type="image/png" sizes="32x32" href="/path/to/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="96x96" href="/path/to/favicon-96x96.png">
```

- [All About Favicons (And Touch Icons)](https://bitsofco.de/all-about-favicons-and-touch-icons/)
- [Favicon Cheat Sheet](https://github.com/audreyr/favicon-cheat-sheet)

## Social

### Facebook Open Graph

``` html
<meta property="fb:app_id" content="123456789">
<meta property="og:url" content="https://example.com/page.html">
<meta property="og:type" content="website">
<meta property="og:title" content="Content Title">
<meta property="og:image" content="https://example.com/image.jpg">
<meta property="og:description" content="Description Here">
<meta property="og:site_name" content="Site Name">
<meta property="og:locale" content="en_US">
<meta property="article:author" content="">
```

- [Facebook Open Graph Markup](https://developers.facebook.com/docs/sharing/webmasters#markup)
- [Open Graph protocol](http://ogp.me/)

### Facebook Instant Articles

``` html
<meta charset="utf-8">
<meta property="op:markup_version" content="v1.0">

<!-- The URL of the web version of your article -->
<link rel="canonical" href="http://example.com/article.html">

<!-- The style to be used for this article -->
<meta property="fb:article_style" content="myarticlestyle">
```

- [Facebook Instant Articles: Creating Articles](https://developers.facebook.com/docs/instant-articles/guides/articlecreate)
- [Instant Articles: Format Reference](https://developers.facebook.com/docs/instant-articles/reference)

### Twitter Cards

``` html
<meta name="twitter:card" content="summary">
<meta name="twitter:site" content="@site_account">
<meta name="twitter:creator" content="@individual_account">
<meta name="twitter:url" content="https://example.com/page.html">
<meta name="twitter:title" content="Content Title">
<meta name="twitter:description" content="Content description less than 200 characters">
<meta name="twitter:image" content="https://example.com/image.jpg">
```

- [Twitter Cards: Getting Started Guide](https://dev.twitter.com/cards/getting-started)
- [Twitter Card Validator](https://cards-dev.twitter.com/validator)

### Google+ / Schema.org

``` html
<link href="https://plus.google.com/+YourPage" rel="publisher">
<meta itemprop="name" content="Content Title">
<meta itemprop="description" content="Content description less than 200 characters">
<meta itemprop="image" content="https://example.com/image.jpg">
```

### Pinterest

Pinterest lets you prevent people from saving things from your website, according [to their help center](https://help.pinterest.com/en/articles/prevent-people-saving-things-pinterest-your-site). The `description` is optional.

``` html
<meta name="pinterest" content="nopin" description="Sorry, you can't save from my website!">
```

### OEmbed

``` html
<link rel="alternate" type="application/json+oembed"
  href="http://example.com/services/oembed?url=http%3A%2F%2Fexample.com%2Ffoo%2F&amp;format=json"
  title="oEmbed Profile: JSON">
<link rel="alternate" type="text/xml+oembed"
  href="http://example.com/services/oembed?url=http%3A%2F%2Fexample.com%2Ffoo%2F&amp;format=xml"
  title="oEmbed Profile: XML">
```

- [oEmbed format](http://oembed.com/)

## Browsers / Platforms

### Apple iOS

``` html
<!-- Smart App Banner -->智能应用banner
<!-- 智能应用banner -->
<meta name="apple-itunes-app" content="app-id=APP_ID,affiliate-data=AFFILIATE_ID,app-argument=SOME_TEXT">

<!-- Disable automatic detection and formatting of possible phone numbers -->
<!-- 禁用自动检测和格式化可能的电话号码 -->
<meta name="format-detection" content="telephone=no">

<!-- Add to Home Screen -->
<!-- 添加到主屏 -->
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black">
<meta name="apple-mobile-web-app-title" content="App Title">

<!-- Touch Icons -->
<!-- 触摸图标 -->
<!-- In most cases, one 180×180px touch icon in the head is enough -->
<!-- 在大多数情况下，180x180px触摸图标在head内足够啦 -->
<link rel="apple-touch-icon" href="/path/to/apple-touch-icon.png">
<!-- Note: Safari on iOS 7 doesn’t add effects to icons. -->
<!-- 注意：ios7上的safari不会对icon添加效果 -->
<!-- Older versions of Safari will not add effects for icon files named with the -precomposed.png suffix. -->
<!-- 老版本的safari不会添加icon文件命名与-precomposed.png后缀效应 -->

<!-- Startup Image ( Deprecated ) -->
<!-- 启动图片(不推荐使用) -->
<link rel="apple-touch-startup-image" href="/path/to/startup.png">

<!-- iOS app deep linking -->
<!-- ios应用深度链接 -->
<meta name="apple-itunes-app" content="app-id=APP-ID, app-argument=http/url-sample.com">
<link rel="alternate" href="ios-app://APP-ID/http/url-sample.com">
```

- [Apple Meta Tags](https://developer.apple.com/library/safari/documentation/AppleApplications/Reference/SafariHTMLRef/Articles/MetaTags.html)

### Apple Safari

```html
<!-- Pinned Site -->
<!-- 固定站点 -->
<link rel="mask-icon" href="/path/to/icon.svg" color="red">
```

### Google Android

``` html
<meta name="theme-color" content="#E64545">

<!-- Add to home screen -->
<!-- 添加到主屏 -->
<meta name="mobile-web-app-capable" content="yes">
<!-- More info: https://developer.chrome.com/multidevice/android/installtohomescreen -->

<!-- Android app deep linking -->
<!-- 安卓应用深度链接 -->
<meta name="google-play-app" content="app-id=package-name">
<link rel="alternate" href="android-app://package-name/http/url-sample.com">
```

### Google Chrome

``` html
<link rel="chrome-webstore-item" href="https://chrome.google.com/webstore/detail/APP_ID">

<!-- Disable translation prompt -->
<!-- 关闭快速翻译 -->
<meta name="google" content="notranslate">
```
### Google Chrome Mobile (Android Only)

Since Chrome 31, you can set up your web app to "app mode" like Safari.

``` html
<!-- Link to a manifest and define the manifest metadata. -->
<!-- 链接到manifest，并定义manifest单元数据 -->
<!-- The example of manifest.json could be found in the link below. -->
<!-- manifest.json的例子能在链接下面被找到 -->
<link rel="manifest" href="manifest.json">

<!-- Define your web page as a web app -->
<!-- 将web页定义为web应用 -->
<meta name="mobile-web-app-capable" content="yes">

<!-- Homescreen Icon  -->
<!-- 首屏图标 -->
<link rel="icon" sizes="192x192" href="highres-icon.png">
```

- [Google Developer](https://developer.chrome.com/multidevice/android/installtohomescreen)

### Microsoft Internet Explorer

``` html
<meta http-equiv="x-ua-compatible" content="ie=edge">
<meta name="skype_toolbar" content="skype_toolbar_parser_compatible">

<!-- IE10: Disable link highlighting upon tap (https://blogs.windows.com/buildingapps/2012/11/15/adapting-your-webkit-optimized-site-for-internet-explorer-10/) -->
<!-- ie10: 禁用链接高亮显示 -->
<meta name="msapplication-tap-highlight" content="no">

<!-- Pinned sites (https://msdn.microsoft.com/en-us/library/dn255024(v=vs.85).aspx) -->
<meta name="application-name" content="Sample Title">
<meta name="msapplication-tooltip" content="A description of what this site does.">
<meta name="msapplication-starturl" content="http://example.com/index.html?pinned=true">
<meta name="msapplication-navbutton-color" content="#FF3300">
<meta name="msapplication-window" content="width=800;height=600">
<meta name="msapplication-task" content="name=Task 1;action-uri=http://host/Page1.html;icon-uri=http://host/icon1.ico">
<meta name="msapplication-task" content="name=Task 2;action-uri=http://microsoft.com/Page2.html;icon-uri=http://host/icon2.ico">
<meta name="msapplication-badge" value="frequency=NUMBER_IN_MINUTES;polling-uri=http://example.com/path/to/file.xml">
<meta name="msapplication-TileColor" content="#FF3300">
<meta name="msapplication-TileImage" content="/path/to/tileimage.jpg">

<meta name="msapplication-config" content="http://example.com/browserconfig.xml">
<meta name="msapplication-notification" content="frequency=60;polling-uri=http://example.com/livetile;polling-uri2=http://example.com/livetile2">
<meta name="msapplication-task-separator" content="1">
```

## App Links

``` html
<!-- iOS -->
<meta property="al:ios:url" content="applinks://docs">
<meta property="al:ios:app_store_id" content="12345">
<meta property="al:ios:app_name" content="App Links">
<!-- Android -->
<meta property="al:android:url" content="applinks://docs">
<meta property="al:android:app_name" content="App Links">
<meta property="al:android:package" content="org.applinks">
<!-- Web Fallback -->
<meta property="al:web:url" content="http://applinks.org/documentation">
<!-- More info: http://applinks.org/documentation/ -->
```

- [App Links Docs](http://applinks.org/documentation/)

## Browsers (Chinese)

### 360 Browser

``` html
<!-- select rendering engine in order -->
<!-- 按顺序选择渲染引擎 -->
<meta name="renderer" content="webkit|ie-comp|ie-stand">
```

### QQ Mobile Browser

``` html
<!-- Locks the screen into the specified orientation -->
<!-- 将屏幕锁定到指定方向 -->
<meta name="x5-orientation" content="landscape/portrait">
<!-- Display this page in fullscreen -->
<!-- 全屏显示此页 -->
<meta name="x5-fullscreen" content="true">
<!-- Page will be displayed in "application mode"(fullscreen,etc.) -->
<!-- 页面将在"应用模式（全屏等）"显示 -->
<meta name="x5-page-mode" content="app">
```

### UC Mobile Browser

``` html
<!-- Locks the screen into the specified orientation -->
<!-- 将屏幕锁定到指定方向 -->
<meta name="screen-orientation" content="landscape/portrait">
<!-- Display this page in fullscreen -->
<!-- 在全屏显示此页 -->
<meta name="full-screen" content="yes">
<!-- UC browser will display images even if in "text mode" -->
<!-- UC浏览器将显示图片即便是在"文本模式" -->
<meta name="imagemode" content="force">
<!-- Page will be displayed in "application mode"(fullscreen,forbiding gesture, etc.) -->
<!-- 页面将被显示在 "应用模式(全屏，禁止手势，等)" -->
<meta name="browsermode" content="application">
<!-- Disabled the UC browser's "night mode" in this page -->
<!-- 在本页禁用uc浏览器 "夜间模式" -->
<meta name="nightmode" content="disable">
<!-- Simplify the page to reduce data transfer -->
<!-- 简化页面以减少数据传输 -->
<meta name="layoutmode" content="fitscreen">
<!-- Disable the UC browser's feature of "scaling font up when there are many words in this page" -->
<!-- 禁用UC浏览器的功能：当页面有很多单词时缩放字体 -->
<meta name="wap-font-scale" content="no">
```

- [UC Browser Docs](http://www.uc.cn/download/UCBrowser_U3_API.doc)

## Notes

### Performance 性能
Moving the `href` attribute to the beginning of an element improves compression when GZIP is enabled, because the `href` attribute is used in `a`, `base` and `link` tags.

移动href属性到元素前，提高压缩gzip的启用，因为href属性被用于a,base和link标签

Example:

``` html
<link href="https://fonts.googleapis.com/css?family=Open+Sans:400,700" rel="stylesheet">
```

## Other Resources

- [HTML5 Boilerplate Docs: The HTML](https://github.com/h5bp/html5-boilerplate/blob/master/dist/doc/html.md)
- [HTML5 Boilerplate Docs: Extend and customize](https://github.com/h5bp/html5-boilerplate/blob/master/dist/doc/extend.md)

## Related Projects

- [Atom HTML Head Snippets](https://github.com/joshbuchea/atom-html-head-snippets) - Atom package for `HEAD` snippets
- [Sublime Text HTML Head Snippets](https://github.com/marcobiedermann/sublime-head-snippets) - Sublime Text package for `HEAD` snippets
- [head-it](https://github.com/hemanth/head-it) - CLI interface for `HEAD` snippets
- [vue-head](https://github.com/ktquez/vue-head) - Manipulating the meta information of the `HEAD` tag for Vue.js

## Other Formats

- [PDF](https://gitprint.com/joshbuchea/HEAD/blob/master/README.md)

## Translations

- [Brazilian Portuguese](https://github.com/Webschool-io/HEAD)
- [Chinese (Simplified)](https://github.com/Amery2010/HEAD)
- [Italian](https://github.com/Fakkio/HEAD)
- [Japanese](http://coliss.com/articles/build-websites/operation/work/collection-of-html-head-elements.html)
- [Russian/Русский](https://github.com/Konfuze/HEAD)
- [Turkish/Türkçe](https://github.com/mkg0/HEAD)

## Contributing

**Open an issue or a pull request to suggest changes or additions.**

### Guide

The **HEAD** repository consists of two branches:

#### 1. `master`

This branch consists of the `README.md` file that is automatically reflected on the [\<head> Cheat Sheet](http://gethead.info/) website. All changes to the content of the cheat sheet as such should be directed to this file.

Please follow these steps for pull requests:

- Modify only one tag, or one related set of tags at a time
- Use double quotes on attributes
- Don't include a trailing slash in self-closing elements — the HTML5 spec says they're optional
- Consider including a link to documentation that supports your change

#### 2. `gh-pages`

This branch is responsible for the [\<head> Cheat Sheet](http://gethead.info/) website. We use [Jekyll](https://jekyllrb.com/) to deploy the `README.md` Markdown file through [GitHub Pages](https://pages.github.com/). All website related modifications must be directed here.

You might want to go through the [Jekyll Docs](https://jekyllrb.com/docs/home/) and understand how Jekyll works before working on this branch.

### Contributors

Check out all the super awesome [contributors](https://github.com/joshbuchea/HEAD/graphs/contributors).

## Author

**[Josh Buchea](http://joshbuchea.com/)**

## License

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Josh Buchea](http://joshbuchea.com) has waived all copyright and related or neighboring rights to this work.
