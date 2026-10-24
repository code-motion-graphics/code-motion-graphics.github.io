---
title: 不具合と対応
---
# 不具合と対応

ご報告いただいた不具合と、直した内容です。直したものは、AI に「CODE MOTION GRAPHICS を更新して」と言えば反映されます。

{% if site.data.fixes.size == 0 %}<p class="lead">いまのところ、ご報告はありません。</p>{% endif %}
{% for x in site.data.fixes %}
<div class="fix" id="{{ x.id }}" markdown="1">
### {{ x.title }}
<span class="meta">{{ x.date }}　{% if x.status == "fixed" %}<span class="tag new">直しました</span>{% elsif x.status == "workaround" %}<span class="tag">回避策あり</span>{% else %}<span class="tag">調査中</span>{% endif %}{% if x.version %}スキル {{ x.version }}{% endif %}</span>

<dl><dt>起きたこと</dt><dd markdown="span">{{ x.symptom }}</dd><dt>原因</dt><dd markdown="span">{{ x.cause }}</dd><dt>対応</dt><dd markdown="span">{{ x.fix }}</dd></dl>
</div>
{% endfor %}
