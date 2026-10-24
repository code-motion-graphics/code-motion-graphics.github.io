---
title: よくある質問
---
# よくある質問

{% assign cats = site.data.faq | map: "category" | uniq %}
{% for c in cats %}
## {{ c }}
{% for f in site.data.faq %}{% if f.category == c %}
<details class="qa" id="{{ f.id }}"><summary>{{ f.q }}</summary><div class="a" markdown="1">
{{ f.a }}

<span class="meta">{{ f.added }}{% if f.source == "form" %}<span class="tag new">ご質問から追加</span>{% endif %}</span>
</div></details>
{% endif %}{% endfor %}
{% endfor %}
