---
title: HTMLMediaElement.playbackRate
slug: Web/API/HTMLMediaElement/playbackRate
tags:
  - API
  - HTML DOM
  - HTMLMediaElement
  - Property
  - プロパティ
translation_of: Web/API/HTMLMediaElement/playbackRate
---
{{APIRef("HTML DOM")}}

**`HTMLMediaElement.playbackRate`** プロパティは、メディアが再生されるレートを設定します。これはユーザーが早送りやスローモーションなどのユーザー制御を実装するために使用されます。通常の再生レートにこの値を掛けて現在のレートが求められるため、 1.0 の値が通常の速度です。

`playbackRate` が負の数であれば、メディアは逆方向に再生されます。

音声は、逆方向の再生であったり、早送りやスロー再生が実用的な範囲を外れていた場合 (例えば、 Gecko は `0.25` から `5.0` の範囲であれば) ミュートされます。

既定では音声の高さが修正され、どの速度でも同じになります。ブラウザーによっては、これを制御するために標準外の `preservespitch` プロパティを実装しています。

<h2 id="Syntax" name="Syntax">構文</h2>

<pre class="brush: js">// 動画
<var>video</var>.playbackRate = 1.5;
// 音声
<var>audio</var>.playbackRate = 1.0;
</pre>

<h3 id="Value" name="Value">値</h3>

`[double](https://en.wikipedia.org/wiki/Double-precision_floating-point_format)` 型。 `1.0` は「通常の速度」で、 `1.0` より小さければ通常より遅く、大きければ通常より早く再生されます。 (**既定値:** `1.0`)

<h2 id="Example" name="Example">例</h2>

<pre class="brush: js">var obj = document.createElement('video');
console.log(obj.playbackRate); // Expected Output: 1</pre>

<h2 id="Specifications" name="Specifications">仕様書</h2>

<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">仕様書</th>
   <th scope="col">状態</th>
   <th scope="col">備考</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>{{SpecName('HTML WHATWG', "#dom-media-playbackrate", "HTMLMediaElement.playbackRate")}}</td>
   <td>{{Spec2('HTML WHATWG')}}</td>
   <td> </td>
  </tr>
  <tr>
   <td>{{SpecName('HTML5 W3C', "embedded-content-0.html#htmlmediaelement", "HTMLMediaElement.playbackRate")}}</td>
   <td>{{Spec2('HTML5 W3C')}}</td>
   <td> </td>
  </tr>
 </tbody>
</table>

<h2 id="Browser_compatibility" name="Browser_compatibility">ブラウザーの対応</h2>

{{Compat("api.HTMLMediaElement.playbackRate")}}

<h2 id="See_also" name="See_also">関連情報</h2>

<ul>
 <li>{{domxref("HTMLMediaElement")}} で定義しています。</li>
</ul>