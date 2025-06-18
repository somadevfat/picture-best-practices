---
# このファイルがJekyllの処理対象であることを示すために記述します。
# titleなどを設定することも推奨されます。
title: ホーム
---

# ページ一覧

<ul>
  {% for page in site.pages %}
    {% if page.title and page.url != "/" %}
      <li><a href="{{ site.baseurl }}{{ page.url }}">{{ page.title }}</a></li>
    {% endif %}
  {% endfor %}
</ul>