{% assign months = "janvier|février|mars|avril|mai|juin|juillet|août|septembre|octobre" | split: "|" %}
{% for month in months %}
{% if forloop.index | trim == page.date | date: "%-m" %}
{% assign current_month = month %}
{% endif %}
{% endfor %}
