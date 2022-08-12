---
title: 图像文件类型与格式指南
slug: Web/Media/Formats/Image_types
tags:
  - 图像
  - 图片
  - 多媒体
  - 指南
  - 文件
  - 文件格式
  - 文件类型
  - 照片
translation_of: Web/Media/Formats/Image_types
---
<div>{{QuickLinksWithSubpages("/zh-CN/docs/Web/Media")}}</div>

<p>在本指南中，我们将介绍网页浏览器普遍支持的图像文件类型，并提供一些关于他们的信息与见解，帮助您为您的网站选择最合适的图像格式。</p>

<h2 id="常见图像文件类型">常见图像文件类型</h2>

<p>世界上有非常多的图像文件格式。下面列举了网页上常用的格式，其中 BMP 由于浏览器支持限制而不被推荐，通常应该避免在网页内容中使用。</p>

<div id="table-of-image-file-types">
<table class="standard-table">
 <thead>
  <tr>
   <th scope="row">缩写</th>
   <th scope="row">文件格式</th>
   <th scope="col">MIME 类型</th>
   <th scope="col">文件拓展名</th>
   <th scope="col">浏览器兼容性</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <th scope="row"><a href="#apng_animated_portable_network_graphics">APNG</a></th>
   <th scope="row">Animated Portable Network Graphics<br>
    <strong>动态便携式网络图像</strong></th>
   <td><code>image/apng</code></td>
   <td><code>.apng</code></td>
   <td>Chrome, Edge, Firefox, Opera, Safari</td>
  </tr>
  <tr>
   <th scope="row"><a href="#avif">AVIF</a></th>
   <th scope="row">AV1 Image File Format<br>
    AV1 图像文件格式</th>
   <td><code>image/avif</code></td>
   <td><code>.avif</code></td>
   <td>Chrome, Opera, Firefox (feature flag)</td>
  </tr>
  <tr>
   <th scope="row"><a href="#bmp_bitmap_file">BMP</a></th>
   <th scope="row">Bitmap file<br>
    <strong>位图</strong>文件</th>
   <td><code>image/bmp</code></td>
   <td><code>.bmp</code></td>
   <td>Chrome, Edge, Firefox, Internet Explorer, Opera, Safari</td>
  </tr>
  <tr>
   <th scope="row"><a href="#gif_graphics_interchange_format">GIF</a></th>
   <th scope="row">Graphics Interchange Format<br>
    图像互换格式</th>
   <td><code>image/gif</code></td>
   <td><code>.gif</code></td>
   <td>Chrome, Edge, Firefox, Internet Explorer, Opera, Safari</td>
  </tr>
  <tr>
   <th scope="row"><a href="#ico_microsoft_windows_icon">ICO</a></th>
   <th scope="row">Microsoft Icon<br>
    微软图标</th>
   <td><code>image/x-icon</code></td>
   <td><code>.ico</code>, <code>.cur</code></td>
   <td>Chrome, Edge, Firefox, Internet Explorer, Opera, Safari</td>
  </tr>
  <tr>
   <th scope="row"><a href="#jpeg_joint_photographic_experts_group_image">JPEG</a></th>
   <th scope="row">Joint Photographic Expert Group image<br>
    联合影像专家小组图像</th>
   <td><code>image/jpeg</code></td>
   <td><code>.jpg</code>, <code>.jpeg</code>, <code>.jfif</code>, <code>.pjpeg</code>, <code>.pjp</code></td>
   <td>Chrome, Edge, Firefox, Internet Explorer, Opera, Safari</td>
  </tr>
  <tr>
   <th scope="row"><a href="#png_portable_network_graphics">PNG</a></th>
   <th scope="row">Portable Network Graphics<br>
    <strong>便携式网络图像</strong></th>
   <td><code>image/png</code></td>
   <td><code>.png</code></td>
   <td>Chrome, Edge, Firefox, Internet Explorer, Opera, Safari</td>
  </tr>
  <tr>
   <th scope="row"><a href="#svg_scalable_vector_graphics">SVG</a></th>
   <th scope="row">Scalable Vector Graphics<br>
    <strong>可缩放矢量图形</strong></th>
   <td><code>image/svg+xml</code></td>
   <td><code>.svg</code></td>
   <td>Chrome, Edge, Firefox, Internet Explorer, Opera, Safari</td>
  </tr>
  <tr>
   <th scope="row"><a href="#tiff_tagged_image_file_format">TIFF</a></th>
   <th scope="row">Tagged Image File Format<br>
    标签图像文件格式</th>
   <td><code>image/tiff</code></td>
   <td><code>.tif</code>, <code>.tiff</code></td>
   <td>Safari</td>
  </tr>
  <tr>
   <th scope="row"><a href="#webp_image">WebP</a></th>
   <th scope="row">Web Picture format<br>
    万维网图像格式</th>
   <td><code>image/webp</code></td>
   <td><code>.webp</code></td>
   <td>Chrome, Edge, Firefox, Opera, Safari</td>
  </tr>
 </tbody>
</table>

<p>每一种格式缩写都有一个详细说明，其功能以及详细的浏览器兼容信息， 包括哪个版本引入支持以及以后可能会引入的特殊功能。</p>
</div>

<h2 id="图像文件格式详介">图像文件格式详介</h2>

<p>The following sections provide a brief overview of each of the image file types supported by web browsers.</p>

<p>In the tables below, the term <strong>bits per component</strong> refers to the number of bits used to represent each color component. For example, an RGB color depth of 8 indicates that each of the red, green, and blue components are represented by an 8-bit value. <strong>Bit depth</strong>, on the other hand, is the total number of bits used to represent each pixel in memory.</p>

<h3 id="APNG_Animated_Portable_Network_Graphics"><a id="APNG" name="APNG">APNG</a> (Animated Portable Network Graphics)</h3>

<p>APNG is a file format first introduced by Mozilla which extends the <a href="#png_portable_network_graphics">PNG</a> standard to add support for animated images. Conceptually similar to the animated GIF format which has been in use for decades, APNG is more capable in that it supports a variety of <a href="https://zh.wikipedia.org/wiki/color_depth">color depths</a>, whereas animated GIF supports only 8-bit <a href="https://zh.wikipedia.org/wiki/indexed_color">indexed color</a>.</p>

<p>APNG is ideal for basic animations that do not need to synchronize to other activities or to a sound track, such as progress indicators, activity <a href="https://zh.wikipedia.org/wiki/throbber">throbbers</a>, and other animated sequences. For example, APNG is <a href="https://developer.apple.com/stickers/">one of the formats supported when creating animated stickers</a> for Apple's iMessage application (and the Messages application on iOS). They're also commonly used for the animated portions of web browsers' user interfaces.</p>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="row">MIME 类型</th>
   <td><code>image/apng</code></td>
  </tr>
  <tr>
   <th scope="row">文件拓展名</th>
   <td><code>.apng</code></td>
  </tr>
  <tr>
   <th scope="row">规范</th>
   <td><a href="https://wiki.mozilla.org/APNG_Specification">wiki.mozilla.org/APNG_Specification</a></td>
  </tr>
  <tr>
   <th scope="row">浏览器兼容性</th>
   <td>Chrome 59, Edge 12, Firefox 3, Opera 46, Safari 8</td>
  </tr>
  <tr>
   <th scope="row">最高分辨率</th>
   <td>2,147,483,647×2,147,483,647 pixels</td>
  </tr>
  <tr>
   <th scope="row">支持的颜色模式</th>
   <td>
    <table class="standard-table">
     <thead>
      <tr>
       <th scope="row">颜色模式</th>
       <th scope="col">Bits per component (<em>D</em>)</th>
       <th scope="col">描述</th>
      </tr>
     </thead>
     <tbody>
      <tr>
       <th scope="row">Greyscale</th>
       <td>1, 2, 4, 8, and 16</td>
       <td>Each pixel consists of a single <em>D</em>-bit value indicating the brightness of the greyscale pixel.</td>
      </tr>
      <tr>
       <th scope="row">True color</th>
       <td>8 and 16</td>
       <td>Each pixel is represented by three <em>D</em>-bit values indicating the level of the red, green, and blue color components.</td>
      </tr>
      <tr>
       <th scope="row">Indexed color</th>
       <td>1, 2, 4, and 8</td>
       <td>Each pixel is a <em>D</em>-bit value indicating an index into a color palette which is contained within a <code><a href="https://www.w3.org/TR/PNG/#11PLTE">PLTE</a></code> chunk in the APNG file; the colors in the palette all use an 8-bit depth.</td>
      </tr>
      <tr>
       <th scope="row">Greyscale with alpha</th>
       <td>8 and 16</td>
       <td>Each pixel is represented by two <em>D</em>-bit values: the intensity of the greyscale pixel and an alpha sample, indicating how opaque the pixel is.</td>
      </tr>
      <tr>
       <th scope="row">True color with alpha</th>
       <td>8 and 16</td>
       <td>Each pixel is comprised of four <em>D</em>-pixel color components: red, green, blue, and the alpha sample indicating how opaque the pixel is.</td>
      </tr>
     </tbody>
    </table>
   </td>
  </tr>
  <tr>
   <th scope="row">压缩</th>
   <td>Lossless</td>
  </tr>
  <tr>
   <th scope="row">授权</th>
   <td>Free and open under the <a href="http://creativecommons.org/licenses/by-sa/3.0/">Creative Commons Attribution-ShareAlike license</a> (<a href="http://creativecommons.org/licenses/by-sa/3.0/">CC-BY-SA</a>) version 3.0 or later.</td>
  </tr>
 </tbody>
</table>

<h3 id="BMP_Bitmap_file"><a id="BMP" name="BMP">BMP</a> (Bitmap file)</h3>

<p>The <strong>BMP</strong> (<strong>Bitmap image</strong>) file type is most prevalent on Windows computers, and is generally used only for special cases in web apps and content.</p>

<div class="blockIndicator warning">
<p><strong>Note:</strong> You should typically avoid using BMP for web site content, as it's not a generally-accepted use of the format.</p>
</div>

<p>BMP theoretically supports a variety of internal data representations. The simplest, and most commonly used, form of BMP file is an uncompressed raster image, with each pixel occupying 3 bytes representing its red, green, and blue components, and each row padded with <code>0x00</code> bytes to a multiple of 4 bytes wide.</p>

<p>While other data representations are defined in the specification, they are not widely used and often completely unimplemented. These features include: support for different bit depths, indexed color, alpha channels, and different pixel orders (by default, BMP is written from bottom-left corner toward the right and top, rather than from the top-left corner toward the right and bottom).</p>

<p>Theoretically, several compression algorithms are supported, and the image data can also be stored in <a href="#jpeg_joint_photographic_experts_group_image">JPEG</a> or <a href="#png_portable_network_graphics">PNG</a> format within the BMP file.</p>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="row">MIME 类型</th>
   <td><code>image/bmp</code></td>
  </tr>
  <tr>
   <th scope="row">文件拓展名</th>
   <td><code>.bmp</code></td>
  </tr>
  <tr>
   <th scope="row">规范</th>
   <td>No specification; however, Microsoft provides general documentation of the format at <a href="https://docs.microsoft.com/en-us/windows/desktop/gdi/bitmap-storage">docs.microsoft.com/en-us/windows/desktop/gdi/bitmap-storage</a></td>
  </tr>
  <tr>
   <th scope="row">浏览器兼容性</th>
   <td>All versions of Chrome, Edge, Firefox, Internet Explorer, Opera, and Safari</td>
  </tr>
  <tr>
   <th scope="row">最高分辨率</th>
   <td>Either 32,767×32,767 or 2,147,483,647×2,147,483,647 pixels, depending on the format version</td>
  </tr>
  <tr>
   <th scope="row">支持的颜色模式</th>
   <td>
    <table class="standard-table">
     <thead>
      <tr>
       <th scope="row">颜色模式</th>
       <th scope="col">Bits per component (<em>D</em>)</th>
       <th scope="col">描述</th>
      </tr>
     </thead>
     <tbody>
      <tr>
       <th scope="row">Greyscale</th>
       <td>1</td>
       <td>Each bit represents a single pixel, which can be either black or white.</td>
      </tr>
      <tr>
       <th scope="row">True color</th>
       <td>8 and 16</td>
       <td>Each pixel is represented by three values representing the red, green, and blue color components; each is <em>D</em> bits.</td>
      </tr>
      <tr>
       <th scope="row">Indexed color</th>
       <td>2, 4, and 8</td>
       <td>Each pixel is represented by a value which is one 2, 4, or 8 bits, serving as an index into the color table.</td>
      </tr>
      <tr>
       <th scope="row">Greyscale with alpha</th>
       <td><em>n/a</em></td>
       <td>BMP has no distinct grayscale format.</td>
      </tr>
      <tr>
       <th scope="row">True color with alpha</th>
       <td>8 and 16</td>
       <td>Each pixel is represented by four values representing the red, green, blue, and alpha color components; each is <em>D</em> bits.</td>
      </tr>
     </tbody>
    </table>
   </td>
  </tr>
  <tr>
   <th scope="row">压缩</th>
   <td>Several compression methods are supported, including lossy or lossless algorithms</td>
  </tr>
  <tr>
   <th scope="row">授权</th>
   <td>Covered by the <a href="https://docs.microsoft.com/en-us/openspecs/dev_center/ms-devcentlp/1c24c7c8-28b0-4ce1-a47d-95fe1ff504bc">Microsoft Open Specification Promise</a>; while Microsoft holds patents against BMP, they have published a promise not to assert its patent rights as long as specific conditions are met. This is not the same as a license, however. BMP is included under the Windows Metafile Format (<code>.wmf</code>).</td>
  </tr>
 </tbody>
</table>

<h3 id="GIF_Graphics_Interchange_Format"><a id="GIF" name="GIF">GIF</a> (Graphics Interchange Format)</h3>

<p>In 1987, the CompuServe online service provider introduced the <strong><a href="https://zh.wikipedia.org/wiki/GIF">GIF</a></strong> (<strong>Graphics Interchange Format</strong>) image file format to provide a compressed graphics format that all members of their service would be able to use. GIF uses the <a href="https://zh.wikipedia.org/wiki/Lempel-Ziv-Welch">Lempel-Ziv-Welch</a> (LZW) algorithm to losslessly compress 8-bit indexed color graphics. GIF was one of the first two graphics formats supported by {{Glossary("HTML")}}, along with <a href="#xbm_x_window_system_bitmap_file">XBM</a>.</p>

<p>Each pixel in a GIF is represented by a single 8-bit value serving as an index into a palette of 24-bit colors (8 bits each of red, green, and blue). The length of a color table is always a power of 2 (that is, each palette has 2, 4, 8, 16, 32, 64, or 256 entries). To simulate more than 255 or 256 colors, <a href="https://zh.wikipedia.org/wiki/dithering">dithering</a> is generally used. It is <a href="https://gif.ski/">technically possible</a> to tile multiple image blocks, each with its own color palette, to create truecolor images, but in practice this is rarely done.</p>

<p>Pixels are opaque, unless a specific color index is designated as transparent, in which case pixels colored that value are entirely transparent.</p>

<p>GIF supports simple animation, in which following an initial full-size frame, a series of images reflecting the parts of the image that change with each frame are provided.</p>

<p>GIF has been extremely popular for decades, due to its simplicity and compatibility. Its animation support caused a resurgence in its popularity in the social media era, when animated GIFs began to be widely used for short "videos", memes, and other simple animation sequences.</p>

<p>Another popular feature of GIF is support for <a href="https://zh.wikipedia.org/wiki/Interlacing_(bitmaps)">interlacing</a>, where rows of pixels are stored out of order so that partially-received files can be displayed in lower quality. This is particularly useful when network connections are slow.</p>

<p>GIF is a good choice for simple images and animations, although converting full color images to GIF can result in unsatisfactory dithering. Typically, modern content should use <a href="#png_portable_network_graphics">PNG</a> for lossless <em>and</em> indexed still images, and should consider using <a href="#apng_animated_portable_network_graphics">APNG</a> for lossless animation sequences.</p>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="row">MIME 类型</th>
   <td><code>image/gif</code></td>
  </tr>
  <tr>
   <th scope="row">文件拓展名</th>
   <td><code>.gif</code></td>
  </tr>
  <tr>
   <th scope="row">规范</th>
   <td><a href="https://www.w3.org/Graphics/GIF/spec-gif87.txt">GIF87a specification</a><br>
    <a href="https://www.w3.org/Graphics/GIF/spec-gif89a.txt">GIF89a specification</a></td>
  </tr>
  <tr>
   <th scope="row">浏览器兼容性</th>
   <td>All versions of Chrome, Edge, Firefox, Internet Explorer, Opera, and Safari</td>
  </tr>
  <tr>
   <th scope="row">最高分辨率</th>
   <td>65,536×65,536 pixels</td>
  </tr>
  <tr>
   <th scope="row">支持的颜色模式</th>
   <td>
    <table class="standard-table">
     <thead>
      <tr>
       <th scope="row">颜色模式</th>
       <th scope="col">Bits per component (<em>D</em>)</th>
       <th scope="col">描述</th>
      </tr>
     </thead>
     <tbody>
      <tr>
       <th scope="row">Greyscale</th>
       <td><em>n/a</em></td>
       <td>GIF does not include a dedicated greyscale format.</td>
      </tr>
      <tr>
       <th scope="row">True color</th>
       <td><em>n/a</em></td>
       <td>GIF does not support true color pixels.</td>
      </tr>
      <tr>
       <th scope="row">Indexed color</th>
       <td>8</td>
       <td>Each color in a GIF palette is defined as 8 bits each of red, green, and blue (24 total bits per pixel).</td>
      </tr>
      <tr>
       <th scope="row">Greyscale with alpha</th>
       <td><em>n/a</em></td>
       <td>GIF does not provide a dedicated greyscale format.</td>
      </tr>
      <tr>
       <th scope="row">True color with alpha</th>
       <td><em>n/a</em></td>
       <td>GIF does not support true color pixels.</td>
      </tr>
     </tbody>
    </table>
   </td>
  </tr>
  <tr>
   <th scope="row">压缩</th>
   <td>Lossless (LZW)</td>
  </tr>
  <tr>
   <th scope="row">授权</th>
   <td>While the GIF format itself is open, the LZW compression algorithm was covered by patents until the early 2000s. As of July 7, 2004, all relevant patents have expired and the GIF format may be used freely</td>
  </tr>
 </tbody>
</table>

<h3 id="ICO_Microsoft_Windows_icon"><a id="ICO" name="ICO">ICO</a> (Microsoft Windows icon)</h3>

<p>The ICO (Microsoft Windows icon) file format was designed by Microsoft for desktop icons of Windows systems. However, early versions of Internet Explorer introduced the ability for a web site to provide a ICO file named <code>favicon.ico</code> in a web site's root directory to specify a <strong><a href="/zh-CN/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML#Adding_custom_icons_to_your_site">favicon</a></strong> — an icon to be displayed in the Favorites menu, and other places where an iconic representation of the site would be useful.</p>

<p>An ICO file can contain multiple icons, and begins with a directory listing details about each. Following the directory comes the data for the icons. Each icon's data can be either a <a href="#bmp_bitmap_file">BMP</a> image without the file header, or a complete <a href="#png_portable_network_graphics">PNG</a> image (including the file header). If you use ICO files, you should use the BMP format, as support for PNG inside ICO files wasn't added until Windows Vista and may not be well supported.</p>

<div class="blockIndicator warning">
<p>ICO files <em>should not</em> be used in web content. Additionally, their use for favicons has subsided in favor of using a PNG file and the {{HTMLElement("link")}} element, as described in {{SectionOnPage("/en-US/docs/Web/HTML/Element/link", "Providing icons for different usage contexts")}}.</p>
</div>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="row">MIME 类型</th>
   <td><code>image/vnd.microsoft.icon</code> (official), <code>image/x-icon</code> (used by Microsoft)</td>
  </tr>
  <tr>
   <th scope="row">文件拓展名</th>
   <td><code>.ico</code></td>
  </tr>
  <tr>
   <th scope="row">规范</th>
   <td></td>
  </tr>
  <tr>
   <th scope="row">浏览器兼容性</th>
   <td>All versions of Chrome, Edge, Firefox, Internet Explorer, Opera, and Safari</td>
  </tr>
  <tr>
   <th scope="row">最高分辨率</th>
   <td>256×256 pixels</td>
  </tr>
  <tr>
   <th scope="row">支持的颜色模式</th>
   <td>
    <table class="standard-table">
     <caption>Icons in BMP format</caption>
     <tbody>
      <tr>
       <th scope="row">颜色模式</th>
       <th scope="col">Bits per component (<em>D</em>)</th>
       <th scope="col">描述</th>
      </tr>
      <tr>
       <th scope="row">Greyscale</th>
       <td>1</td>
       <td>Each bit represents a single pixel, which can be either black or white.</td>
      </tr>
      <tr>
       <th scope="row">True color</th>
       <td>8 and 16</td>
       <td>Each pixel is represented by three values representing the red, green, and blue color components; each is <em>D</em> bits.</td>
      </tr>
      <tr>
       <th scope="row">Indexed color</th>
       <td>2, 4, and 8</td>
       <td>Each pixel is represented by a value which is one 2, 4, or 8 bits, serving as an index into the color table.</td>
      </tr>
      <tr>
       <th scope="row">Greyscale with alpha</th>
       <td><em>n/a</em></td>
       <td>BMP has no distinct grayscale format.</td>
      </tr>
      <tr>
       <th scope="row">True color with alpha</th>
       <td>8 and 16</td>
       <td>Each pixel is represented by four values representing the red, green, blue, and alpha color components; each is <em>D</em> bits.</td>
      </tr>
     </tbody>
    </table>

    <table class="standard-table">
     <caption>Icons in PNG format</caption>
     <tbody>
      <tr>
       <th scope="row">颜色模式</th>
       <th scope="col">Bits per component (<em>D</em>)</th>
       <th scope="col">描述</th>
      </tr>
      <tr>
       <th scope="row">Greyscale</th>
       <td>1, 2, 4, 8, and 16</td>
       <td>Each pixel consists of a single <em>D</em>-bit value indicating the brightness of the greyscale pixel.</td>
      </tr>
      <tr>
       <th scope="row">True color</th>
       <td>8 and 16</td>
       <td>Each pixel is represented by three <em>D</em>-bit values indicating the level of the red, green, and blue color components.</td>
      </tr>
      <tr>
       <th scope="row">Indexed color</th>
       <td>1, 2, 4, and 8</td>
       <td>Each pixel is a <em>D</em>-bit value indicating an index into a color palette which is contained within a <code><a href="https://www.w3.org/TR/PNG/#11PLTE">PLTE</a></code> chunk in the APNG file; the colors in the palette all use an 8-bit depth.</td>
      </tr>
      <tr>
       <th scope="row">Greyscale with alpha</th>
       <td>8 and 16</td>
       <td>Each pixel is represented by two <em>D</em>-bit values: the intensity of the greyscale pixel and an alpha sample, indicating how opaque the pixel is.</td>
      </tr>
      <tr>
       <th scope="row">True color with alpha</th>
       <td>8 and 16</td>
       <td>Each pixel is comprised of four <em>D</em>-pixel color components: red, green, blue, and the alpha sample indicating how opaque the pixel is.</td>
      </tr>
     </tbody>
    </table>
   </td>
  </tr>
  <tr>
   <th scope="row">压缩</th>
   <td>BMP-format icons nearly always use lossless compression, but lossy methods are available. PNG icons are always compressed losslessly.</td>
  </tr>
  <tr>
   <th scope="row">授权</th>
   <td>—</td>
  </tr>
 </tbody>
</table>

<h3 id="JPEG_Joint_Photographic_Experts_Group_image"><a id="JPEG" name="JPEG">JPEG</a> (Joint Photographic Experts Group image)</h3>

<p>The {{Glossary("JPEG")}} (typically pronounced "<strong>jay-peg</strong>") image format is currently the most widely used lossy compression format for still images. It's particulary useful for photographs; applying lossy compression to content requiring sharpness, like diagrams or charts, can produce unsatisfactory results.</p>

<p>JPEG is actually a data format for compressed photos, rather than a file type. The JFIF (<strong>J</strong>PEG <strong>F</strong>ile <strong>I</strong>nterchange <strong>F</strong>ormat) specification describes the format of the files we think of as "JPEG" images.</p>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="row">MIME 类型</th>
   <td><code>image/jpeg</code></td>
  </tr>
  <tr>
   <th scope="row">文件拓展名</th>
   <td><code>.jpg</code>, <code>.jpeg</code>, <code>.jpe</code>, <code>.jif</code>, <code>.jfif</code></td>
  </tr>
  <tr>
   <th scope="row">规范</th>
   <td><a href="https://jpeg.org/jpeg/">jpeg.org/jpeg/</a></td>
  </tr>
  <tr>
   <th scope="row">浏览器兼容性</th>
   <td>All versions of Chrome, Edge, Firefox, Internet Explorer, Opera, and Safari</td>
  </tr>
  <tr>
   <th scope="row">最高分辨率</th>
   <td>65,535×65,535 pixels</td>
  </tr>
  <tr>
   <th scope="row">支持的颜色模式</th>
   <td>
    <table class="standard-table">
     <thead>
      <tr>
       <th scope="row">颜色模式</th>
       <th scope="col">Bits per component (<em>D</em>)</th>
       <th scope="col">描述</th>
      </tr>
     </thead>
     <tbody>
      <tr>
       <th scope="row">Greyscale</th>
       <td><em>n/a</em></td>
       <td>JPEG has no distinct greyscale mode.</td>
      </tr>
      <tr>
       <th scope="row">True color</th>
       <td>8</td>
       <td>Each pixel is described by the red, blue, and green color components, each of which is 8 bits.</td>
      </tr>
      <tr>
       <th scope="row">Indexed color</th>
       <td><em>n/a</em></td>
       <td>JPEG does not offer an indexed color mode.</td>
      </tr>
      <tr>
       <th scope="row">Greyscale with alpha</th>
       <td><em>n/a</em></td>
       <td>JPEG does not support an alpha channel.</td>
      </tr>
      <tr>
       <th scope="row">True color with alpha</th>
       <td><em>n/a</em></td>
       <td>JPEG does not support an alpha channel.</td>
      </tr>
     </tbody>
    </table>
   </td>
  </tr>
  <tr>
   <th scope="row">压缩</th>
   <td>Lossy; based on the <a href="https://zh.wikipedia.org/wiki/discrete_cosine_transform">discrete cosine transform</a></td>
  </tr>
  <tr>
   <th scope="row">授权</th>
   <td>As of October 27, 2006, all United States patents have expired.</td>
  </tr>
 </tbody>
</table>

<h3 id="PNG_Portable_Network_Graphics"><a id="PNG" name="PNG">PNG</a> (Portable Network Graphics)</h3>

<p>The {{Glossary("PNG")}} (pronounced "<strong>ping</strong>") image format uses lossless or lossy compression to provide more efficient compression, and supports higher color depths than <a href="#gif_graphics_interchange_format">GIF</a>, as well as full alpha transparency support.</p>

<p>PNG is widely supported, with all major browsers offering full support for its features. Internet Explorer, which introduced PNG support in versions 4–5, did not fully support it until IE 9, and had many infamous bugs for many of the intervening years, including in the once-omnipresent Internet Explorer 6. This slowed PNG adoption, but it is now commonly used, especially when precise reproduction of the source image is needed.</p>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="row">MIME 类型</th>
   <td><code>image/png</code></td>
  </tr>
  <tr>
   <th scope="row">文件拓展名</th>
   <td><code>.png</code></td>
  </tr>
  <tr>
   <th scope="row">规范</th>
   <td><a href="https://www.w3.org/TR/PNG">w3.org/TR/PNG</a></td>
  </tr>
  <tr>
   <th scope="row">浏览器兼容性</th>
   <td>
    <table class="standard-table">
     <thead>
      <tr>
       <th scope="row">Feature</th>
       <th scope="col">Chrome</th>
       <th scope="col">Edge</th>
       <th scope="col">Firefox</th>
       <th scope="col">Internet Explorer</th>
       <th scope="col">Opera</th>
       <th scope="col">Safari</th>
      </tr>
     </thead>
     <tbody>
      <tr>
       <th scope="row">Basic support</th>
       <td>1</td>
       <td>12</td>
       <td>1</td>
       <td>5</td>
       <td>3.5.1 (Presto)<br>
        15 (Blink)</td>
       <td>1</td>
      </tr>
      <tr>
       <th scope="row">Alpha channel</th>
       <td>1</td>
       <td>12</td>
       <td>1</td>
       <td>5</td>
       <td>6 (Presto)<br>
        All (Blink)</td>
       <td>1</td>
      </tr>
      <tr>
       <th scope="row">Gamma correction</th>
       <td>no</td>
       <td>yes</td>
       <td>1</td>
       <td>8</td>
       <td>1</td>
       <td>broken</td>
      </tr>
      <tr>
       <th scope="row">Color correction</th>
       <td>no</td>
       <td>yes</td>
       <td>3</td>
       <td>9</td>
       <td>no</td>
       <td>no</td>
      </tr>
      <tr>
       <th scope="row">Interlacing</th>
       <td>no</td>
       <td>?</td>
       <td>1</td>
       <td>broken</td>
       <td>3.5.1</td>
       <td>no</td>
      </tr>
     </tbody>
    </table>
   </td>
  </tr>
  <tr>
   <th scope="row">最高分辨率</th>
   <td>2,147,483,647×2,147,483,647 pixels</td>
  </tr>
  <tr>
   <th scope="row">支持的颜色模式</th>
   <td>
    <table class="standard-table">
     <thead>
      <tr>
       <th scope="row">颜色模式</th>
       <th scope="col">Bits per component (<em>D</em>)</th>
       <th scope="col">描述</th>
      </tr>
     </thead>
     <tbody>
      <tr>
       <th scope="row">Greyscale</th>
       <td>1, 2, 4, 8, and 16</td>
       <td>Each pixel consists of a single <em>D</em>-bit value indicating the brightness of the greyscale pixel.</td>
      </tr>
      <tr>
       <th scope="row">True color</th>
       <td>8 and 16</td>
       <td>Each pixel is represented by three <em>D</em>-bit values indicating the level of the red, green, and blue color components.</td>
      </tr>
      <tr>
       <th scope="row">Indexed color</th>
       <td>1, 2, 4, and 8</td>
       <td>Each pixel is a <em>D</em>-bit value indicating an index into a color palette which is contained within a <code><a href="https://www.w3.org/TR/PNG/#11PLTE">PLTE</a></code> chunk in the APNG file; the colors in the palette all use an 8-bit depth.</td>
      </tr>
      <tr>
       <th scope="row">Greyscale with alpha</th>
       <td>8 and 16</td>
       <td>Each pixel is represented by two <em>D</em>-bit values: the intensity of the greyscale pixel and an alpha sample, indicating how opaque the pixel is.</td>
      </tr>
      <tr>
       <th scope="row">True color with alpha</th>
       <td>8 and 16</td>
       <td>Each pixel is comprised of four <em>D</em>-pixel color components: red, green, blue, and the alpha sample indicating how opaque the pixel is.</td>
      </tr>
     </tbody>
    </table>
   </td>
  </tr>
  <tr>
   <th scope="row">压缩</th>
   <td>Lossless, optionally indexed color like GIF</td>
  </tr>
  <tr>
   <th scope="row">授权</th>
   <td>©2003 <a href="https://www.w3.org/">W3C</a><sup>®</sup> (<a href="http://www.lcs.mit.edu/">MIT</a>, <a href="http://www.ercim.org/">ERCIM</a>, <a href="http://www.keio.ac.jp/">Keio</a>), All Rights Reserved. W3C <a href="http://www.w3.org/Consortium/Legal/ipr-notice#Legal_Disclaimer">liability</a>, <a href="http://www.w3.org/Consortium/Legal/ipr-notice#W3C_Trademarks">trademark</a>, <a href="http://www.w3.org/Consortium/Legal/copyright-documents">document use</a> and <a href="http://www.w3.org/Consortium/Legal/copyright-software">software licensing</a> rules apply. No known royalty-bearing patents.</td>
  </tr>
 </tbody>
</table>

<h3 id="SVG_Scalable_Vector_Graphics"><a id="SVG" name="SVG">SVG</a> (Scalable Vector Graphics)</h3>

<p>SVG is an <a href="/zh-CN/docs/Glossary/XML">XML</a>-based <a href="https://zh.wikipedia.org/wiki/vector_graphics">vector graphics</a> format that specifies the contents of an image as a set of drawing commands that create shapes, lines, apply colors, filters, and so forth. SVG files are ideal for diagrams, icons, and other images which can be accurately drawn at any size. As such, SVG is popular for user interface elements in modern Web design.</p>

<p>SVG files are text files containing source code that, when interpreted, draws the desired image. For instance, this example defines an drawing area with initial size 100 by 100 units, containing a line drawn diagonally through the box:</p>

<pre class="brush: html notranslate">&lt;svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg"&gt;
  &lt;line x1="0" y1="80" x2="100" y2="20" stroke="black" /&gt;
&lt;/svg&gt;</pre>

<p>SVG can be used in web content in two ways:</p>

<ol>
 <li>You can directly write the {{HTMLElement("svg")}} element within the HTML, containing <a href="/zh-CN/docs/Web/SVG/Element">SVG elements</a> to draw the image.</li>
 <li>You can display an SVG image anywhere you can use any of the other image types, including with the {{HTMLElement("img")}} and {{HTMLElement("picture")}} elements, the {{cssxref("background-image")}} CSS property, and so forth.</li>
</ol>

<p>SVG is an ideal choice for images which can be represented using a series of drawing commands, especially if the size at which the image will be rendered is unknown or may vary, since SVG will smoothly scale to the desired size. It's not generally useful for strictly bitmap or photographic images, although it is possible to include bitmap images within an SVG.</p>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="row">MIME 类型</th>
   <td><code>image/svg+xml</code></td>
  </tr>
  <tr>
   <th scope="row">文件拓展名</th>
   <td><code>.svg</code></td>
  </tr>
  <tr>
   <th scope="row">规范</th>
   <td><a href="https://www.w3.org/TR/SVG2">w3.org/TR/SVG2</a></td>
  </tr>
  <tr>
   <th scope="row">浏览器兼容性</th>
   <td>
    <table class="standard-table">
     <thead>
      <tr>
       <th scope="row">Feature</th>
       <th scope="col">Chrome</th>
       <th scope="col">Edge</th>
       <th scope="col">Firefox</th>
       <th scope="col">Internet Explorer</th>
       <th scope="col">Opera</th>
       <th scope="col">Safari</th>
      </tr>
     </thead>
     <tbody>
      <tr>
       <th scope="row">SVG support</th>
       <td>4</td>
       <td>12</td>
       <td>3</td>
       <td>9</td>
       <td>10 (Presto)<br>
        15 (Blink)</td>
       <td>3.2</td>
      </tr>
      <tr>
       <th scope="row">SVG as image ({{HTMLElement("img")}} etc)</th>
       <td>28</td>
       <td>12</td>
       <td>4</td>
       <td>9</td>
       <td>10 (Presto)<br>
        15 (Blink)</td>
       <td>9</td>
      </tr>
     </tbody>
    </table>
   </td>
  </tr>
  <tr>
   <th scope="row">最高分辨率</th>
   <td>无限制</td>
  </tr>
  <tr>
   <th scope="row">支持的颜色模式</th>
   <td>Colors in SVG are specified using <a href="/zh-CN/docs/Web/CSS/color_value">CSS color syntax</a>.</td>
  </tr>
  <tr>
   <th scope="row">压缩</th>
   <td>SVG source may be compressed during transit using <a href="/zh-CN/docs/Web/HTTP/Compression">HTTP compression</a> techniques, or on disk as an <code>.svgz</code> file.</td>
  </tr>
  <tr>
   <th scope="row">授权</th>
   <td>©2018 <a href="https://www.w3.org/">W3C</a><sup>®</sup> (<a href="http://www.lcs.mit.edu/">MIT</a>, <a href="http://www.ercim.org/">ERCIM</a>, <a href="http://www.keio.ac.jp/">Keio</a>, <a href="http://ev.buaa.edu.cn/">Beihang</a>), All Rights Reserved. W3C <a href="http://www.w3.org/Consortium/Legal/ipr-notice#Legal_Disclaimer">liability</a>, <a href="http://www.w3.org/Consortium/Legal/ipr-notice#W3C_Trademarks">trademark</a>, <a href="http://www.w3.org/Consortium/Legal/copyright-documents">document use</a> and <a href="http://www.w3.org/Consortium/Legal/copyright-software">software licensing</a> rules apply. No known royalty-bearing patents.</td>
  </tr>
 </tbody>
</table>

<h3 id="TIFF_Tagged_Image_File_Format"><a id="TIFF" name="TIFF">TIFF</a> (Tagged Image File Format)</h3>

<p><a href="https://zh.wikipedia.org/wiki/TIFF">TIFF</a> is a raster graphics file format which was created to store scanned photos, although it can be any kind of image. It is a somewhat "heavy" format, in that TIFF files have a tendency to be larger than images in other formats. This is because of the metadata often included, as well as the fact that most TIFF images are either uncompressed or use compression algorithms that still leave fairly large files after compression.</p>

<p>TIFF supports a variety of compression methods, but the most commonly used are the CCITT Group 4 (and, for older fax systems, Group 3) compression systems used for by fax software, as well as LZW and lossy JPEG compression.</p>

<p>Every value in a TIFF file is specified using its <strong>tag</strong> (indicating what kind of information it is, such as the width of the image) and its <strong>type</strong> (indicating the format the data is stored in), followed by the length of the array of values to assign to that tag (all properties are stored in arrays, even for single values). This allows different data types to be used for the same properties. For example, the width of an image, <code>ImageWidth</code>, is stored using tag <code>0x0100</code>, and is a one-entry array. By specifying type 3 (<code>SHORT</code>), the value of <code>ImageWidth</code> is stored as a 16-bit value:</p>

<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">Tag</th>
   <th scope="col">Type</th>
   <th scope="col">Size</th>
   <th scope="col">Value</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><code>0x0100</code><br>
    (<code>ImageWidth</code>)</td>
   <td><code>0x0003</code><br>
    (<code>SHORT</code>)</td>
   <td><code>0x00000001</code><br>
    (1 entry)</td>
   <td><code>0x0280</code><br>
    (640 pixels)</td>
  </tr>
 </tbody>
</table>

<p>Specifying type 4 (<code>LONG</code>) stores the width as a 32-bit value:</p>

<table class="standard-table">
 <thead>
  <tr>
   <th scope="col">Tag</th>
   <th scope="col">Type</th>
   <th scope="col">Size</th>
   <th scope="col">Value</th>
  </tr>
  <tr>
   <td><code>0x0100</code><br>
    (<code>ImageWidth</code>)</td>
   <td><code>0x0004</code><br>
    (<code>LONG</code>)</td>
   <td><code>0x00000001</code><br>
    (1 entry)</td>
   <td><code>0x00000280</code><br>
    (640 pixels)</td>
  </tr>
 </thead>
</table>

<p>A single TIFF file can contain multiple images; this may be used to represent multi-page documents, for example (such as a multi-page scanned document, or a received fax). However, software reading TIFF files is only required to support the first image.</p>

<p>TIFF supports a variety of color spaces, not just RGB. These include CMYK, YCbCr, and others, making TIFF a good choice for storing images intended for print, film, or television media.</p>

<p>Long ago, some browsers supported TIFF images in web content; today, however, you need to use special libraries or browser add-ons to do so. As such, TIFF files are not useful within the context of web content, <em>but </em>it's common to provide downloadable TIFF files when distributing photos and other artwork intended for precision editing or printing.</p>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="row">MIME 类型</th>
   <td><code>image/tiff</code></td>
  </tr>
  <tr>
   <th scope="row">文件拓展名</th>
   <td><code>.tif</code>, <code>.tiff</code></td>
  </tr>
  <tr>
   <th scope="row">规范</th>
   <td><a href="https://www.adobe.io/open/standards/TIFF.html">adobe.io/open/standards/TIFF.html</a></td>
  </tr>
  <tr>
   <th scope="row">浏览器兼容性</th>
   <td>No browsers integrate support for TIFF; its value is as a download format</td>
  </tr>
  <tr>
   <th scope="row">最高分辨率</th>
   <td>4,294,967,295×4,294,967,295 pixels (theoretical)</td>
  </tr>
  <tr>
   <th scope="row">支持的颜色模式</th>
   <td>
    <table class="standard-table">
     <tbody>
      <tr>
       <th scope="row">颜色模式</th>
       <th scope="col">Bits per component (<em>D</em>)</th>
       <th scope="col">描述</th>
      </tr>
      <tr>
       <th scope="row">Bilevel</th>
       <td>1</td>
       <td>A bilevel TIFF stores 8 bits in each byte, one bit per pixel. The <code>PhotometricInterpretation</code> field specifies which of 0 and 1 are black and which is white.</td>
      </tr>
      <tr>
       <th scope="row">Greyscale</th>
       <td>4 and 8</td>
       <td>Each pixel consists of a single <em>D</em>-bit value indicating the brightness of the greyscale pixel.</td>
      </tr>
      <tr>
       <th scope="row">True color</th>
       <td>8</td>
       <td>All true color RGB images are stored using 8-bits each of red, green, and blue.</td>
      </tr>
      <tr>
       <th scope="row">Indexed color</th>
       <td>4 and 8</td>
       <td>Each pixel is an index into a <code>ColorMap</code> record, which defines the colors used in the image. The color map lists all of the red values, then all of the green values, then all of the blue values (rather than <code>rgb, rgb, rgb...</code>).</td>
      </tr>
      <tr>
       <th scope="row">Greyscale with alpha</th>
       <td>4 and 8</td>
       <td>Alpha information is added by specifying that there are more than 3 samples per pixel in the <code>SamplesPerPixel</code> field, and indicating the type of alpha (1 for an associated, pre-multiplied alpha component, and 2 for unassociated alpha (a separate matte); however, alpha channels are rarely used in TIFF files and may be unsupported by the user's software.</td>
      </tr>
      <tr>
       <th scope="row">True color with alpha</th>
       <td>8</td>
       <td>Alpha information is added by specifying that there are more than 3 samples per pixel in the <code>SamplesPerPixel</code> field, and indicating the type of alpha (1 for an associated, pre-multiplied alpha component, and 2 for unassociated alpha (a separate matte); however, alpha channels are rarely used in TIFF files and may be unsupported by the user's software.</td>
      </tr>
     </tbody>
    </table>
   </td>
  </tr>
  <tr>
   <th scope="row">压缩</th>
   <td>Most TIFF files are uncompressed, but lossless PackBits and LZW compression are supported, as is lossy JPEG compression.</td>
  </tr>
  <tr>
   <th scope="row">授权</th>
   <td>No license required (aside from any associated with libraries you might use); all known patents have expired.</td>
  </tr>
 </tbody>
</table>

<h3 id="WebP_image"><a id="WebP" name="WebP">WebP image</a></h3>

<p>WebP supports lossy compression via predictive coding based on the VP8 video codec, and lossless compression that uses substitutions for repeating data. Lossy WebP images average 25–35% smaller than JPEG images of visually similar compression levels. Lossless WebP images are typically 26% smaller than the same images in PNG format.</p>

<p>WebP also supports animation: in a lossy WebP file, the image data is represented by a VP8 bitstream, which may contain multiple frames. Lossless WebP holds the <code>ANIM</code> chunk, which describes the animation, and the <code>ANMF</code> chunk, which represents a frame of an animation sequence. Looping is supported.</p>

<p>WebP now has broad support in the latest versions of major web browsers, although it does not have deep historical support. Provide a fallback in either <a href="#jpeg_joint_photographic_experts_group_image">JPEG</a> or <a href="#png_portable_network_graphics">PNG</a> format, such as with <a href="/zh-CN/docs/Web/HTML/Element/picture">the <code>&lt;picture&gt;</code> element</a>.</p>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="row">MIME 类型</th>
   <td><code>image/webp</code></td>
  </tr>
  <tr>
   <th scope="row">文件拓展名</th>
   <td><code>.webp</code></td>
  </tr>
  <tr>
   <th scope="row">规范</th>
   <td>
    <p><a href="https://developers.google.com/speed/webp/docs/riff_container">RIFF Container Specification</a><br>
     {{RFC(6386, "VP8 Data Format and Decoding Guide")}} (lossy encoding)<br>
     <a href="https://developers.google.com/speed/webp/docs/webp_lossless_bitstream_specification">WebP Lossless Bitstream Specification</a></p>
   </td>
  </tr>
  <tr>
   <th scope="row">浏览器兼容性</th>
   <td>
    <table class="standard-table">
     <tbody>
      <tr>
       <th scope="row">Feature</th>
       <th scope="col">Chrome</th>
       <th scope="col">Edge</th>
       <th scope="col">Firefox</th>
       <th scope="col">Internet Explorer</th>
       <th scope="col">Opera</th>
       <th scope="col">Safari</th>
      </tr>
      <tr>
       <th scope="row">Lossy WebP support</th>
       <td>17</td>
       <td>18</td>
       <td>65</td>
       <td>no</td>
       <td>11.10 (Presto)<br>
        15 (Blink)</td>
       <td>no</td>
      </tr>
      <tr>
       <th scope="row">Lossless WebP</th>
       <td>23<br>
        25 on Android</td>
       <td>18</td>
       <td>65</td>
       <td>no</td>
       <td>12.10 (Presto)<br>
        15 (Blink)</td>
       <td>no</td>
      </tr>
      <tr>
       <th scope="row">动画</th>
       <td>32</td>
       <td>18</td>
       <td>65</td>
       <td>no</td>
       <td>19 (Blink)</td>
       <td>no</td>
      </tr>
     </tbody>
    </table>
   </td>
  </tr>
  <tr>
   <th scope="row">最高分辨率</th>
   <td>16,383×16,383 pixels</td>
  </tr>
  <tr>
   <th scope="row">支持的颜色模式</th>
   <td>Lossy WebP stores the image in 8-bit Y'CbCr 4:2:0 (YUV420) format. Lossless WebP uses 8-bit ARGB color, with each component taking 8 bits for a total of 32 bits per pixel.</td>
  </tr>
  <tr>
   <th scope="row">压缩</th>
   <td>Lossless (Huffman, LZ77, or color cache codes) or lossy (VP8).</td>
  </tr>
  <tr>
   <th scope="row">授权</th>
   <td>No license required; source code is openly available.</td>
  </tr>
 </tbody>
</table>

<h3 id="XBM_X_Window_System_Bitmap_file"><a id="XBM" name="XBM">XBM</a> (X Window System Bitmap file)</h3>

<p>XBM (X Bitmap) files were the first to be supported on the Web, but are no longer used and should be avoided, as their format has potential security concerns. Modern browsers have not supported XBM files in many years, but when dealing with older content, you may find some still around.</p>

<p>XBM uses a snippet of C code to represent the contents of the image as an array of bytes. Each image consists of 2 to 4 <code>#define</code> directives, providing the width and height of the bitmap (and optionally the hotspot, if the image is designed as a cursor), followed by an array of <code>unsigned char</code>, where each value contains 8 1-bit monochrome pixels.</p>

<p>The image must be a multiple of 8 pixels wide. For example, the following code represents an XBM image which is 8 pixels by 8 pixels, with those pixels in a black-and-white checkerboard pattern:</p>

<pre class="brush: cpp notranslate">#define square8_width 8
#define square8_height 8
static unsigned char square8_bits[] = {
  0xAA, 0x55, 0xAA, 0x55, 0xAA, 0x55, 0xAA, 0x55
};
</pre>

<table class="standard-table">
 <tbody>
  <tr>
   <th scope="row">MIME 类型</th>
   <td><code>image/xbm</code>, <code>image-xbitmap</code></td>
  </tr>
  <tr>
   <th scope="row">文件拓展名</th>
   <td><code>.xbm</code></td>
  </tr>
  <tr>
   <th scope="row">规范</th>
   <td>None</td>
  </tr>
  <tr>
   <th scope="row">浏览器兼容性</th>
   <td>Firefox 1–3.5, Internet Explorer 1–5</td>
  </tr>
  <tr>
   <th scope="row">最高分辨率</th>
   <td>无限制</td>
  </tr>
  <tr>
   <th scope="row">支持的颜色模式</th>
   <td>
    <table class="standard-table">
     <thead>
      <tr>
       <th scope="row">颜色模式</th>
       <th scope="col">Bits per component</th>
       <th scope="col">描述</th>
      </tr>
     </thead>
     <tbody>
      <tr>
       <th scope="row">Greyscale</th>
       <td>1</td>
       <td>Each byte contains eight 1-bit pixels.</td>
      </tr>
      <tr>
       <th scope="row">True color</th>
       <td><em>n/a</em></td>
       <td><em>n/a</em></td>
      </tr>
      <tr>
       <th scope="row">Indexed color</th>
       <td><em>n/a</em></td>
       <td><em>n/a</em></td>
      </tr>
      <tr>
       <th scope="row">Greyscale with alpha</th>
       <td><em>n/a</em></td>
       <td><em>n/a</em></td>
      </tr>
      <tr>
       <th scope="row">True color with alpha</th>
       <td><em>n/a</em></td>
       <td><em>n/a</em></td>
      </tr>
     </tbody>
    </table>
   </td>
  </tr>
  <tr>
   <th scope="row">压缩</th>
   <td>Lossless</td>
  </tr>
  <tr>
   <th scope="row">授权</th>
   <td>Open source</td>
  </tr>
 </tbody>
</table>

<h2 id="选择合适的图像格式">选择合适的图像格式</h2>

<p>Picking the best image format for your needs is likely easier than video formats, as there are fewer options with broad support, and each tends to have a specific set of use-cases.</p>

<h3 id="Photographs">Photographs</h3>

<p>Photographs typically fare well with lossy compression (depending on the encoder's configuration). This makes <a href="#jpeg_joint_photographic_experts_group_image">JPEG</a> and <a href="#webp_image">WebP</a> good choices for photographs, with JPEG being more compatible but WebP perhaps offering better compression. To maximize quality and minimize download time, consider providing both <a href="#提供后备图像">using a fallback</a> with WebP as the first choice and JPEG as the second. Otherwise, JPEG is the safe choice for compatibility.</p>

<table class="standard-table" style="max-width: 42rem;">
 <thead>
  <tr>
   <th scope="col" style="width: 50%;">Best choice</th>
   <th scope="col">Fallback</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>WebP or JPEG</td>
   <td>JPEG</td>
  </tr>
 </tbody>
</table>

<h3 id="Icons">Icons</h3>

<p>For smaller images such as icons, use a lossless format to avoid loss of detail in a size-constrained image. While lossless WebP is ideal for this purpose, support is not widespread yet, so PNG is a better choice unless you offer a <a href="#提供后备图像">fallback</a>. If your image contains fewer than 256 colors, GIF is an option, although PNG often compresses even smaller with its indexed compression option (PNG-8).</p>

<p>If the icon can be represented using vector graphics, consider <a href="#svg_scalable_vector_graphics">SVG</a>, since it scales across various resolutions and sizes, so it's perfect for responsive design. Although SVG support is good, it may be worth offering a PNG fallback for older browsers.</p>

<table class="standard-table" style="max-width: 42rem;">
 <thead>
  <tr>
   <th scope="col" style="width: 50%;">Best choice</th>
   <th scope="col">Fallback</th>
  </tr>
  <tr>
   <td>SVG, Lossless WebP, or PNG</td>
   <td>PNG</td>
  </tr>
 </thead>
</table>

<h3 id="Screenshots">Screenshots</h3>

<p>Unless you're willing to compromise on quality, you should use a lossless format for screenshots. This is particularly important if there's any text in your screenshot, as text easily becomes fuzzy and unclear under lossy compression.</p>

<p>PNG is probably your best bet, but lossless WebP is arguably going to be better compressed.</p>

<table class="standard-table" style="max-width: 42rem;">
 <thead>
  <tr>
   <th scope="col" style="width: 50%;">Best choice</th>
   <th scope="col">Fallback</th>
  </tr>
  <tr>
   <td>Lossless WebP or PNG;<br>
    JPEG if compression artifacts aren't a concern</td>
   <td>PNG or JPEG;<br>
    GIF for screenshots with low color counts</td>
  </tr>
 </thead>
</table>

<h3 id="Diagrams_drawings_and_charts">Diagrams, drawings, and charts</h3>

<p>For any image that can be represented using vector graphics, SVG is the best choice. Otherwise, you should use a lossless format like PNG. If you do choose a lossy format, such as JPEG or lossy WebP, carefully weigh the compression level to avoid causing text or other shapes to become fuzzy or unclear.</p>

<table class="standard-table" style="max-width: 42rem;">
 <thead>
  <tr>
   <th scope="col" style="width: 50%;">Best choice</th>
   <th scope="col">Fallback</th>
  </tr>
  <tr>
   <td><a href="#svg_scalable_vector_graphics">SVG</a></td>
   <td><a href="#png_portable_network_graphics">PNG</a></td>
  </tr>
 </thead>
</table>

<h2 id="提供后备图像">提供后备图像</h2>

<p>While the standard HTML {{HTMLElement("img")}} element doesn't support compatibility fallbacks for images, the {{HTMLElement("picture")}} element does. <code>&lt;picture&gt;</code> is used as a wrapper for a number of {{HTMLElement("source")}} elements, each specifying a version of the image in a different format or under different <a href="/zh-CN/docs/Web/CSS/@media">media conditions</a>, as well as an <code>&lt;img&gt;</code> element which defines where to display the image and the fallback to the default or "most compatible" version.</p>

<p>For example, if you're displaying a diagram best displayed with SVG, but wish to offer a fallback to a PNG or GIF of the diagram, you would do something like this:</p>

<pre class="brush: html notranslate">&lt;picture&gt;
  &lt;source srcset="diagram.svg" type="image/svg+xml"&gt;
  &lt;source srcset="diagram.png" type="image/png"&gt;
  &lt;img src="diagram.gif" width="620" height="540"
       alt="Diagram showing the data channels"&gt;
&lt;/picture&gt;
</pre>

<p>You can specify as many <code>&lt;source&gt;</code>s as you wish, though typically 2 or 3 is all you need.</p>

<h2 id="参见">参见</h2>

<ul>
 <li><a href="/zh-CN/docs/Web/Media/Formats">Guide to media types and formats</a></li>
 <li><a href="/zh-CN/docs/Web/Media">Web media technologies</a></li>
 <li><a href="/zh-CN/docs/Web/Media/Formats/Video_codecs">Guide to video codecs used on the web</a></li>
 <li>The {{Glossary("HTML")}} {{HTMLElement("img")}} and {{HTMLElement("picture")}} elements</li>
 <li>The CSS {{cssxref("background-image")}} property</li>
 <li>The {{domxref("Image()")}} constructor and the {{domxref("HTMLImageElement")}} interface</li>
</ul>