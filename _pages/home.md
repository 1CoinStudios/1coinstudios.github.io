---
layout: single
permalink: /
hidden: true
header:
  overlay_image: /assets/images/splash.jpg
  actions:
    - label: "<i class='fas fa-download'></i> Download"
      url: "https://assetstore.unity.com/publishers/36858"
---

{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
  {% for post in collection.docs %}
    {% unless collection.output == false or collection.label == "posts" %}
      {% include archive-single.html %}
    {% endunless %}
  {% endfor %}
{% endfor %}