<center><h1>破解批改网<del>禁止粘贴, 禁止拖拽</del>的限制,自动填充题目, 禁用<del>时间限制</del>, etc</h1></center>
<hr>
<dl>
  <dd><center>之前的Github账号被莫名其妙封禁, 白瞎了大量的star, 这是新号. 话说美国这是新冠病入膏肓了? 都开始随便封禁帐号了, 服气嗷~~~</center></dd>
<dd>如果觉得本脚本不错的话请给个免费的star~使用前请先仔细看下方介绍, 如果您之前没有接触过用户脚本(user scripts), 请先进行了解 <a href="https://greasyfork.org/zh-CN/help/installing-user-scripts" title="帮助">传送门</a></dd>
</dl>
<ul>
<li>最近有同学问我能不能有强制补交功能, 这个我试了, 是不能的, 模拟请求会被服务器端拒绝, 真要实现只能找漏洞攻击, 不过我也不是什么黑客, 没这个能耐(捂脸)</li><br>
<li><i><b>重要信息: 本脚本仅对<a href="https://www.pigai.org" title="跳转到批改网">批改网</a>有效!一般的网站禁止粘贴都是禁止了paste事件, 而批改网是监视键盘来禁止的粘贴, 比较特殊, 所以我写了这样的一个脚本.</b></i></li><br>
<li><b><mark>重磅功能: 作文评分界面查看相似详情(勿传播, 怕被和谐) ⚠请勿滥用</li></b></mark><br>
<li>相信大部分小伙伴是因为想要避开禁止粘贴所以找到我这个脚本的吧😂别急, 我还加了些别的实用功能</li><br>
<li>使用的是<code>$('#contents').unbind();</code>方法,此方法最简单但是会使字数统计功能失效,因此重新引进字数统计功能, 可以动态统计字数, 如果出现问题请手动点击字数统计按钮(使用的是批改网原版字数统计策略,放心使用)</li><br>
<li><mark>增加各大翻译站链接, 增加直接搜索题目功能(Baidu, Google)</mark></li><br>
<li>亮度调节(Beta), 如果觉得不好请反馈, 我将其去掉或更改</li><br>
<li>去除了一些碍眼的广告和无用的功能(如人工批改)</li><br>
<li>填充标题按钮, 点一下即可自动填充标题</li><br>
<li>如果老师启用了时间限制, 那么会创建禁用按钮, <i>对大多数人没啥用</i></li><br>
<li>关闭网页前自动存草稿, 防止不小心关闭网页导致数据丢失</li><br>
<li>旧版本强制跳转到新版本(可选), 旧版本界面不美观并且功能差, 用户进入旧版本界面往往是因为网站cookie设置错误, 本脚本会对cookie进行修正(<em>这里指的旧版本不是/?c=v1类型的旧版本, 而是url和新版本完全一致但是界面老旧的旧版本)</em></li><br>
<li><b>关于查重: </b>即使批改网不显示重复也可能是重复作文, 因为老师可以设置不让你看见相似提示,请不要抱有侥幸<sub>我就被坑过(小声bb)</sub></li><br>
<li>如果老师没有启用"禁止粘贴",本脚本不会执行相关破解代码</li><br>
<li>火狐, Edge的严格模式会导致外链自定义等重要功能彻底失效</li><br>
<li><b>划重点, 请使用新版PC端批改网, 其他的不做适配</b></li><br>
<li>Adguard 的广告拦截器"Fanboy's Enhanced Tracking List"会导致脚本异常</li><br>
<li>另附批改网写作页面相关的重要js地址: <a href="http://cdn.pigai.org//res/javascript/spss.js">spss.js</a> ,直接用chrome, firefox, edge, opera打开均会乱码, 移动端大部分主流浏览器不会乱码, 建议下载到本地使用utf-8编码查看.&nbsp&nbsp(右键→"Save link as...")</li><br>
<br>
<li>个人用来练手的脚本, 如果有bug请自行更改代码, 也可<a href="https://greasyfork.org/zh-CN/forum/post/discussion?script=393386" target="_blank">反馈</a>或者<a href="https://github.com/consideration-ak/pigaiwang-toolkit/issues">在Github提issue</a>, 反馈时最好带上<b><u>浏览器名称以及版本</u></b>, <b><u>操作系统环境</u></b>, 以及<b><u>控制台信息的截图</u></b>(F12打开控制台后console的内容)</li><br>
<li>代码以<a href="https://spdx.org/licenses/GPL-3.0-only.html?tdsourcetag=s_pctim_aiomsg">GNU General Public License v3.0 only</a>开源</li>
</ul>
<dl>
<dd>效果演示(这是旧版本的截图, 目前的效果请打开批改网自行查看)</dd></dl>
<a href="https://i.loli.net/2020/04/10/pmvrQbhkJSXLP3Z.png"><img src="https://i.loli.net/2020/04/10/pmvrQbhkJSXLP3Z.png"></a>
<dl>
<dl><dd><mark>请我喝杯咖啡</mark></dd></dl><br><img src="https://i.loli.net/2020/04/13/EBpmgMvVLlKFux1.png"</img>
<hr>
<dd><strong>请使用Tampermonkey</a><sup>®</sup>安装脚本, 其他管理器无法正常运行</strong></dd>
<dd><details><summary>Tampermonkey<sup>®</sup>安装途径</summary>
<p><a href="https://www.crx4chrome.com/crx/1429/" title="Tampermonkey's crx file">Crx For Chrome ></a>(crx文件安装方法请自行搜索)</p>
<p><a href="https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo" title="Chrome Web Store">Chrome Web Store ></a></p>
<p><a href="https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/?src=search" title="Firefox ADD-ONS">Firefox ADD-ONS ></a></p>
<p><a href="https://microsoftedge.microsoft.com/insider-addons/detail/iikmkjmpaadaobahmlepeloendndfphd" title="Edge插件">Edge插件 ></a></p>
<p>其他浏览器安装方法请移步Baidu,  Google</p>
</dl>
