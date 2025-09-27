---
weight: 4
title: "Sintaks markdown Dasar"
date: 2025-09-27
lastmod: 2025-09027
draft: false
author: "Aan Triono"
authorLink: "https://www.aantriono.com"
description: "Artikel ini membahas tentang format dan sintaks markdown dasar."
images: []
resources:
- name: "featured-image"
  src: "featured-image.png"

tags: ["Markdown", "HTML"]
categories: ["Markdown"]

lightgallery: true
---

Artikel ini menawarkan contoh sintaks Markdown dasar yang dapat digunakan dalam file konten Hugo.
Catatan

Artikel ini adalah salinan memalukan dari halaman asli Grav yang hebat.

Jika Anda ingin tahu tentang tema Sharpdown sintax of LoveIt yang diperluas, silakan baca halaman sintaks Markdown yang diperpanjang.

Mari kita hadapi itu: Menulis konten untuk Web itu melelahkan. Editor WYSIWYG membantu meringankan tugas ini, tetapi mereka umumnya menghasilkan kode yang mengerikan, atau lebih buruk lagi, halaman web jelek.

Markdown adalah cara yang lebih baik untuk menulis HTMLHTML, tanpa semua kompleksitas dan keburukan yang biasanya menyertainya.

Beberapa manfaat utama adalah:

    Markdown mudah dipelajari, dengan karakter tambahan minimal, jadi juga lebih cepat untuk menulis konten.
    Kurangnya kemungkinan kesalahan saat menulis di Markdown.
    Menghasilkan output XHTML yang valid.
    Menjaga konten dan tampilan visual terpisah, sehingga Anda tidak dapat mengacaukan tampilan situs Anda.
    Tulis di editor teks atau aplikasi Markdown yang Anda sukai.
    Markdown adalah sukacita untuk digunakan!

John Gruber, penulis Markdown, mengatakannya seperti ini:

    Tujuan desain utama untuk sintaks pemformatan Markdown adalah membuatnya dapat dibaca sebisa mungkin. Idenya adalah bahwa dokumen yang diformat Markdown harus dapat dipublikasikan sebagai-adalah, sebagai teks biasa, tanpa terlihat seperti itu telah ditandai dengan tag atau petunjuk pemformatan. Sementara sintaks Markdown telah dipengaruhi oleh beberapa filter teks-ke-HTML yang ada, Satu-satunya sumber inspirasi terbesar untuk sintaks Markdown adalah format email teks biasa.
    - John Gruber

Tanpa penundaan lebih lanjut, mari kita bahas elemen utama Markdown dan seperti apa HTML yang dihasilkan!
Tip
 Bookmark halaman ini untuk memudahkan referensi di masa mendatang!
1 Headings

Judul dari h2 melalui h6 dibangun dengan # Untuk setiap level:

## h2 Heading
### h3 Heading
#### h4 Heading
##### h5 Heading
###### h6 Heading

HTML terlihat seperti ini:

<h2>h2 Heading</h2>
<h3>h3 Heading</h3>
<h4>h4 Heading</h4>
<h5>h5 Heading</h5>
<h6>h6 Heading</h6>

Identitas Heading

Untuk menambahkan ID judul khusus, lampirkan ID khusus dalam kawat gigi keriting pada baris yang sama dengan judul:

### A Great Heading {#custom-id}

HTML terlihat seperti ini:

<h3 id="custom-id">A Great Heading</h3>

2 Komentar

Komentar harus kompatibel dengan HTML.

<!--
This is a comment
-->

Komentar di bawah ini tidak boleh dilihat:
3 Aturan Horizontal

HTML <hr> Elemen adalah untuk menciptakan “tekakan tematik” antara elemen tingkat paragraf. Di Markdown, Anda dapat membuat <hr> dengan salah satu dari berikut:

    ___: tiga underscores berturut-turut
    ---: tiga dasbor berturut-turut
    ***: tiga tanda bintang berturut-turut

Output yang diberikan terlihat seperti ini:
4 Salinan Tubuh

Body copy ditulis sebagai normal, teks biasa akan dibungkus dengan <p></p> tag dalam HTML yang diberikan.

Jadi salinan tubuh ini:

Lorem ipsum dolor sit amet, graecis denique ei vel, at duo primis mandamus. Et legere ocurreret pri,
animal tacimates complectitur ad cum. Cu eum inermis inimicus efficiendi. Labore officiis his ex,
soluta officiis concludaturque ei qui, vide sensibus vim ad.

HTML terlihat seperti ini:

<p>Lorem ipsum dolor sit amet, graecis denique ei vel, at duo primis mandamus. Et legere ocurreret pri, animal tacimates complectitur ad cum. Cu eum inermis inimicus efficiendi. Labore officiis his ex, soluta officiis concludaturque ei qui, vide sensibus vim ad.</p>

Istirahat garis dapat dilakukan dengan satu baris kosong.
5 Inline HTML

Jika Anda membutuhkan tag HTML tertentu (dengan kelas) Anda cukup menggunakan HTML:

Paragraph in Markdown.

<div class="class">
    This is <b>HTML</b>
</div>

Paragraph in Markdown.

6 Penekanan
Berani

Untuk menekankan cuplikan teks dengan berat font yang lebih berat.

Cuplikan teks berikut dianggap sebagai teks yang berani.

**rendered as bold text**
__rendered as bold text__

HTML terlihat seperti ini:

<strong>rendered as bold text</strong>

Italia

Untuk menekankan cuplikan teks dengan huruf miring.

Cuplikan teks berikut ini dianggap sebagai teks yang dicetak miring.

*rendered as italicized text*
_rendered as italicized text_

HTML terlihat seperti ini:

<em>rendered as italicized text</em>

Pemogokan

Dalam GFM Anda dapat melakukan strikethrough.

~~Strike through this text.~~

Output yang diberikan terlihat seperti ini:

Menyerang melalui teks ini.

HTML terlihat seperti ini:

<del>Strike through this text.</del>

Kombinasi

Berani, italics, dan strikethrough dapat digunakan dalam kombinasi.

***bold and italics***
~~**strikethrough and bold**~~
~~*strikethrough and italics*~~
~~***bold, italics and strikethrough***~~

Output yang diberikan terlihat seperti ini:

berani dan italics

Strikethrough dan berani

menyerang dan italics

berani, italics dan strikethrough

HTML terlihat seperti ini:

<em><strong>bold and italics</strong></em>
<del><strong>strikethrough and bold</strong></del>
<del><em>strikethrough and italics</em></del>
<del><em><strong>bold, italics and strikethrough</strong></em></del>

7 Blockquotes

Untuk mengutip blok konten dari sumber lain dalam dokumen Anda.

Tambahkan > sebelum teks apa pun yang ingin Anda kutip:

> **Fusion Drive** combines a hard drive with a flash storage (solid-state drive) and presents it as a single logical volume with the space of both drives combined.

Output yang diberikan terlihat seperti ini:

    Fusion Drive menggabungkan hard drive dengan penyimpanan flash (solid-state drive) dan menyajikannya sebagai volume logis tunggal dengan ruang kedua drive digabungkan.

HTML terlihat seperti ini:

<blockquote>
  <p>
    <strong>Fusion Drive</strong> combines a hard drive with a flash storage (solid-state drive) and presents it as a single logical volume with the space of both drives combined.
  </p>
</blockquote>

Blockquotes juga dapat bersarang:

> Donec massa lacus, ultricies a ullamcorper in, fermentum sed augue.
Nunc augue augue, aliquam non hendrerit ac, commodo vel nisi.
>> Sed adipiscing elit vitae augue consectetur a gravida nunc vehicula. Donec auctor
odio non est accumsan facilisis. Aliquam id turpis in dolor tincidunt mollis ac eu diam.

Output yang diberikan terlihat seperti ini:

    Donec massa lacus, ultricies ullamcorper di, fermentum sed augue. Nunc augugue, alicam non hendrerit ac, commodo vel nisi.

        Sed adipiscing elit vitae augue konsektur a gravida nunc vehicula. Donec austor odio non-est acccumsan facucis. Aliquam id turpis dalam dolor tincidant mollis ac eu diam.

8 Daftar
Tidak Teratur

Daftar item di mana urutan item tidak secara eksplisit penting.

Anda dapat menggunakan salah satu simbol berikut untuk menunjukkan peluru untuk setiap item daftar:

* valid bullet
- valid bullet
+ valid bullet

Sebagai contoh:

* Lorem ipsum dolor sit amet
* Consectetur adipiscing elit
* Integer molestie lorem at massa
* Facilisis in pretium nisl aliquet
* Nulla volutpat aliquam velit
  * Phasellus iaculis neque
  * Purus sodales ultricies
  * Vestibulum laoreet porttitor sem
  * Ac tristique libero volutpat at
* Faucibus porta lacus fringilla vel
* Aenean sit amet erat nunc
* Eget porttitor lorem

Output yang diberikan terlihat seperti ini:

    Lorem ipsum dolor duduk bertemu
    Consecteur adisipsa elit
    Integer molestie lorem di massa
    Facilisis dalam pretium nisl aiquet
    Nulla volutpat aliquam velit
        Phasellus iaculis neque
        Purus sodal ultricies
        Vestibulum laoreet porttitor sem
        Ac tristisque libero volutpat pada
    Faukis porta lacus vel lemparan
    Aenean duduk sebentar terus menerus
    Eget porttitor lorem

HTML terlihat seperti ini:

<ul>
  <li>Lorem ipsum dolor sit amet</li>
  <li>Consectetur adipiscing elit</li>
  <li>Integer molestie lorem at massa</li>
  <li>Facilisis in pretium nisl aliquet</li>
  <li>Nulla volutpat aliquam velit
    <ul>
      <li>Phasellus iaculis neque</li>
      <li>Purus sodales ultricies</li>
      <li>Vestibulum laoreet porttitor sem</li>
      <li>Ac tristique libero volutpat at</li>
    </ul>
  </li>
  <li>Faucibus porta lacus fringilla vel</li>
  <li>Aenean sit amet erat nunc</li>
  <li>Eget porttitor lorem</li>
</ul>

Memesan

Daftar item di mana urutan item secara eksplisit penting.

1. Lorem ipsum dolor sit amet
2. Consectetur adipiscing elit
3. Integer molestie lorem at massa
4. Facilisis in pretium nisl aliquet
5. Nulla volutpat aliquam velit
6. Faucibus porta lacus fringilla vel
7. Aenean sit amet erat nunc
8. Eget porttitor lorem

Output yang diberikan terlihat seperti ini:

    Lorem ipsum dolor duduk bertemu
    Consecteur adisipsa elit
    Integer molestie lorem di massa
    Facilisis dalam pretium nisl aiquet
    Nulla volutpat aliquam velit
    Faukis porta lacus vel lemparan
    Aenean duduk sebentar terus menerus
    Eget porttitor lorem

HTML terlihat seperti ini:

<ol>
  <li>Lorem ipsum dolor sit amet</li>
  <li>Consectetur adipiscing elit</li>
  <li>Integer molestie lorem at massa</li>
  <li>Facilisis in pretium nisl aliquet</li>
  <li>Nulla volutpat aliquam velit</li>
  <li>Faucibus porta lacus fringilla vel</li>
  <li>Aenean sit amet erat nunc</li>
  <li>Eget porttitor lorem</li>
</ol>

Tip

Jika Anda hanya menggunakan 1. untuk setiap nomor, Markdown akan secara otomatis nomor setiap item. Sebagai contoh:

1. Lorem ipsum dolor sit amet
1. Consectetur adipiscing elit
1. Integer molestie lorem at massa
1. Facilisis in pretium nisl aliquet
1. Nulla volutpat aliquam velit
1. Faucibus porta lacus fringilla vel
1. Aenean sit amet erat nunc
1. Eget porttitor lorem

Output yang diberikan terlihat seperti ini:

    Lorem ipsum dolor duduk bertemu
    Consecteur adisipsa elit
    Integer molestie lorem di massa
    Facilisis dalam pretium nisl aiquet
    Nulla volutpat aliquam velit
    Faukis porta lacus vel lemparan
    Aenean duduk sebentar terus menerus
    Eget porttitor lorem

Daftar Tugas

Daftar tugas memungkinkan Anda membuat daftar item dengan kotak centang. Untuk membuat daftar tugas, tambahkan dasbor (-) dan kurung dengan ruang ([ ]) sebelum item daftar tugas. Untuk memilih kotak centang, tambahkan x di antara kurung ([x]).

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

Output yang diberikan terlihat seperti ini:

    Tulis siaran pers
    Perbarui situs web
    Menghubungi media

9 Kode
Kode Inline

Bungkus dalam cuplikan kode dengan `.

In this example, `<section></section>` should be wrapped as **code**.

Output yang diberikan terlihat seperti ini:

Dalam contoh ini, <section></section> harus dibungkus sebagai kode.

HTML terlihat seperti ini:

<p>
  In this example, <code>&lt;section&gt;&lt;/section&gt;</code> should be wrapped with <strong>code</strong>.
</p>

Kode Teridentifikasi

Atau berbagai baris kode dengan setidaknya empat ruang, seperti dalam:

    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code

Output yang diberikan terlihat seperti ini:

// Some comments
line 1 of code
line 2 of code
line 3 of code

HTML terlihat seperti ini:

<pre>
  <code>
    // Some comments
    line 1 of code
    line 2 of code
    line 3 of code
  </code>
</pre>

Blok Kode Berpagar

Gunakan “pagar” ``` untuk memblokir dalam beberapa baris kode dengan atribut bahasa.

```markdown
Sample text here...
```

HTML terlihat seperti ini:

<pre language-html>
  <code>Sample text here...</code>
</pre>

Penyorotan Sintak

GFM juga mendukung penyorotan sintaks.

Untuk mengaktifkannya, cukup tambahkan ekstensi file dari bahasa yang ingin Anda gunakan langsung setelah kode pertama "pagar", ```js, dan sinkped sintaks secara otomatis akan diterapkan dalam HTML yang diberikan.

Misalnya, untuk menerapkan sinkped sintaks ke kode JavaScript:

```js
grunt.initConfig({
  assemble: {
    options: {
      assets: 'docs/assets',
      data: 'src/data/*.{json,yml}',
      helpers: 'src/custom-helpers.js',
      partials: ['src/partials/**/*.{hbs,md}']
    },
    pages: {
      options: {
        layout: 'default.hbs'
      },
      files: {
        './': ['src/templates/pages/index.hbs']
      }
    }
  }
};
```

Output yang diberikan terlihat seperti ini:

grunt.initConfig({
  assemble: {
    options: {
      assets: 'docs/assets',
      data: 'src/data/*.{json,yml}',
      helpers: 'src/custom-helpers.js',
      partials: ['src/partials/**/*.{hbs,md}']
    },
    pages: {
      options: {
        layout: 'default.hbs'
      },
      files: {
        './': ['src/templates/pages/index.hbs']
      }
    }
  }
};

Catatan
Halaman penyorotan sintaksis di Hugo Docs memperkenalkan lebih banyak tentang sorotan sintaks, termasuk toprotan shortcode.
10 Tabel

Tabel dibuat dengan menambahkan pipa sebagai pembagi di antara setiap sel, dan dengan menambahkan garis garis dasbor (juga dipisahkan oleh batang) di bawah header. Perhatikan bahwa pipa tidak perlu disejajarkan secara vertikal.

| Option | Description |
| ------ | ----------- |
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

Output yang diberikan terlihat seperti ini:
Pilihan	Deskripsi
data	path to data file untuk menyediakan data yang akan diteruskan ke template.
mesin	mesin yang akan digunakan untuk template pengolahan. Handlebar adalah default.
yang diekst	ekstensi untuk digunakan untuk file dest.

HTML terlihat seperti ini:

<table>
  <thead>
    <tr>
      <th>Option</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>data</td>
      <td>path to data files to supply the data that will be passed into templates.</td>
    </tr>
    <tr>
      <td>engine</td>
      <td>engine to be used for processing templates. Handlebars is the default.</td>
    </tr>
    <tr>
      <td>ext</td>
      <td>extension to be used for dest files.</td>
    </tr>
  </tbody>
</table>

Teks selaras kanan atau tengah

Menambahkan usus besar di sisi kanan dasbor di bawah judul apa pun akan menyelaraskan teks untuk kolom itu.

Menambahkan usus besar di kedua sisi garis di bawah judul apa pun akan berpusat menyelaraskan teks untuk kolom itu.

| Option | Description |
|:------:| -----------:|
| data   | path to data files to supply the data that will be passed into templates. |
| engine | engine to be used for processing templates. Handlebars is the default. |
| ext    | extension to be used for dest files. |

Output yang diberikan terlihat seperti ini:
Pilihan	Deskripsi
data	path to data file untuk menyediakan data yang akan diteruskan ke template.
mesin	mesin yang akan digunakan untuk template pengolahan. Handlebar adalah default.
yang diekst	ekstensi untuk digunakan untuk file dest.
11 Tautan
Tautan Dasar

<https://assemble.io>
<contact@revolunet.com>
[Assemble](https://assemble.io)

Output yang diberikan terlihat seperti ini (hover di atas tautan, tidak ada tooltip):

https://assemble.io

contact@revolulet.com

Perakitan

HTML terlihat seperti ini:

<a href="https://assemble.io">https://assemble.io</a>
<a href="mailto:contact@revolunet.com">contact@revolunet.com</a>
<a href="https://assemble.io">Assemble</a>

Menambahkan Judul

[Upstage](https://github.com/upstage/ "Visit Upstage!")

Output yang diberikan terlihat seperti ini (hover over the link, harus ada tooltip):

Tahap Atas

HTML terlihat seperti ini:

<a href="https://github.com/upstage/" title="Visit Upstage!">Upstage</a>

Dinamai Jangkar

Jangkar bernama memungkinkan Anda untuk melompat ke titik jangkar yang ditentukan pada halaman yang sama. Sebagai contoh, masing-masing bab ini:

## Table of Contents
  * [Chapter 1](#chapter-1)
  * [Chapter 2](#chapter-2)
  * [Chapter 3](#chapter-3)

akan melompat ke bagian-bagian ini:

## Chapter 1 <a id="chapter-1"></a>
Content for chapter one.

## Chapter 2 <a id="chapter-2"></a>
Content for chapter one.

## Chapter 3 <a id="chapter-3"></a>
Content for chapter one.

Catatan
Penempatan spesifik dari tag jangkar tampaknya sewenang-wenang. Mereka ditempatkan inline di sini karena tampaknya tidak mengganggu, dan itu berhasil.
12 Catatan Kaki

Catatan kaki memungkinkan Anda untuk menambahkan catatan dan referensi tanpa mengacaukan tubuh dokumen. Saat Anda membuat catatan kaki, nomor superskrip dengan tautan muncul di mana Anda menambahkan referensi catatan kaki. Pembaca dapat mengklik tautan untuk melompat ke konten catatan kaki di bagian bawah halaman.

Untuk membuat referensi catatan kaki, tambahkan caret dan pengenal di dalam kurung ([^1]). Pengidentifikasi bisa berupa angka atau kata-kata, tetapi mereka tidak dapat berisi spasi atau tab. Pengidentifikasi hanya menghubungkan referensi catatan kaki dengan catatan kaki itu sendiri - dalam output, catatan kaki diberi nomor secara berurutan.

Tambahkan catatan kaki menggunakan caret lain dan nomor di dalam kurung dengan kolon dan teks ([^1]: My footnote.). Anda tidak perlu menempatkan catatan kaki di akhir dokumen. Anda dapat menempatkan mereka di mana saja kecuali di dalam elemen lain seperti daftar, tandan, dan tabel blok.

This is a digital footnote[^1].
This is a footnote with "label"[^label]

[^1]: This is a digital footnote
[^label]: This is a footnote with "label"

Ini adalah catatan kaki digital 11.

Ini adalah catatan kaki dengan “label” 2
13 Gambar

Gambar memiliki sintaks yang sama dengan tautan tetapi termasuk titik seru sebelumnya.

![Minion](https://octodex.github.com/images/minion.png)

https://octodex.github.com/images/minion.png

atau:

![Alt text](https://octodex.github.com/images/stormtroopocat.jpg "The Stormtroopocat")

https://octodex.github.com/images/stormtroopocat.jpgdari Stormtroopocat

Seperti link, gambar juga memiliki sintaks gaya catatan kaki:

![Alt text][id]

https://octodex.github.com/images/dojocat.jpgUntuk Dojocat

Dengan referensi kemudian dalam dokumen yang menentukan lokasi URL:

[id]: https://octodex.github.com/images/dojocat.jpg  "The Dojocat"

Tip
LoveIt tema memiliki shortcode khusus untuk gambar, yang menyediakan lebih banyak fitur.

    Ini adalah catatan kaki digital ↩

    Ini adalah catatan kaki dengan "label" ↩
