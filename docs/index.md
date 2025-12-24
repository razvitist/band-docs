![Logo](/img/long-mono.svg)

## Браслет, который сделает тебя лучше

Браслет подключается по Wi-Fi и проверяет делаешь ли ты что-нибудь полезное. Если ты не учишься / работаешь / тренируешься, то браслет начинает нагреваться.

---

## Навигация по сайту

{% for item in navigation %}
{% if item.url %}

- [{{ item.title }}]({{ item.url }})

{% else %}

### {{ item.title }}

{% endif %}
{% if item.children %}
{% for child in item.children %}

- [{{ child.title }}]({{ child.url }})

{% endfor %}
{% endif %}
{% endfor %}
