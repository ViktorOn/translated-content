---
title: background_color
slug: Web/Manifest/background_color
translation_of: Web/Manifest/background_color
---
<div>{{QuickLinksWithSubpages("/en-US/docs/Web/Manifest")}}</div>

<table class="properties">
 <tbody>
  <tr>
   <th scope="row">
    <div class="blockIndicator warning">
    <p>wobuhuisuanmin</p>
    </div>

    <h5 id="Type">Type</h5>
   </th>
   <td><code>String</code></td>
  </tr>
  <tr>
   <th scope="row">Mandatory</th>
   <td>No</td>
  </tr>
 </tbody>
</table>

<p>被装载其样式表之前的 <code>background_color</code> 构件限定了用于应用页的占位符的背景颜色来显示。此值用于由用户代理来绘制一个快捷方式的背景颜色，当样式表加载之前清单是可用的。</p>

<p>（原文：The background_color member defines a placeholder background color for the application page to display before its stylesheet is loaded. This value is used by the user agent to draw the background color of a shortcut when the manifest is available before the stylesheet has loaded.）</p>

<p>因此，<code>background_color</code> 应于 {{cssxref("background-color")}}网站样式表中的 CSS 属性匹配，以在启动 Web 应用程序和加载网站内容之间进行平滑过渡。</p>

<p>（原文：Therefore <code>background_color</code> should match the {{cssxref("background-color")}} CSS property in the site’s stylesheet for a smooth transition between launching the web application and loading the site's content.）</p>

<div class="blockIndicator note">
<p><strong>注意</strong>：该 <code>background_color</code> 构件仅用于在从网络或存储介质加载主样式表时改善用户体验。{{cssxref("background-color")}} 当渐进式 Web 应用程序样式表可用时，用户代理不会将其用作 CSS 属性。</p>
</div>

<h2 id="实例">实例</h2>

<pre class="brush: json notranslate">"background_color": "red"</pre>

<h2 id="规范">规范</h2>

{{Specifications}}

<h2 id="浏览器兼容性">浏览器兼容性</h2>

<p>{{Compat}}</p>