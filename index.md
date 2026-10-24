---
title: はじめに
---
# CODE MOTION GRAPHICS 購入者マニュアル

<p class="lead">導入でつまずいたとき、使い方で迷ったときに見るページです。いただいたご質問と不具合のご報告から、毎日更新しています。</p>

<div class="cards">
  <a class="card" href="start/"><b>受け取り・導入</b><span>GitHub の招待から、AI に入れるまで</span></a>
  <a class="card" href="faq/"><b>よくある質問</b><span>{{ site.data.faq | size }}件</span></a>
  <a class="card" href="fixes/"><b>不具合と対応</b><span>報告いただいた不具合と、直した内容</span></a>
  <a class="card" href="updates/"><b>更新履歴</b><span>マニュアルとスキルの更新</span></a>
</div>

## 最近の更新

{% for u in site.data.updates limit:5 %}<div class="log"><span class="meta">{{ u.date }}</span><span class="tag">{% if u.kind == "skill" %}スキル{% else %}マニュアル{% endif %}</span> <b>{{ u.title }}</b><br>{{ u.summary }}</div>
{% endfor %}

## 解決しないときは

このマニュアルで解決しないときは、[質問・不具合報告フォーム](https://forms.gle/JmEkdLW5hhzd6hik8)からお送りください。回答は、個人が分からない形でこのマニュアルに掲載します（通常は翌朝まで）。マニュアルの更新は「購入者通信」でもお知らせします。

## このスキルとの付き合い方

あなたが監督・ディレクターで、スキルは動画クリエイターです。AI にお任せでも動画は完成しますが、0.1秒のこだわりや世界観は、監督の頼み方で変わります。動画生成AIと違って何度でも安く作り直せるので、数を回して試してください。
