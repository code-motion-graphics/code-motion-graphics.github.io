---
title: 更新履歴
---
# 更新履歴

{% for u in site.data.updates %}<div class="log"><span class="meta">{{ u.date }}</span><span class="tag">{% if u.kind == "skill" %}スキル{% else %}マニュアル{% endif %}</span> <b>{{ u.title }}</b><br>{{ u.summary }}</div>
{% endfor %}
