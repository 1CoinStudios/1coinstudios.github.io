---
layout: single
permalink: /
hidden: true
header:
  overlay_image: /assets/images/splash.jpg
  actions:
    - label: "<i class='fas fa-download'></i> Download"
      url: "https://assetstore.unity.com/publishers/36858"

gallery:
  - url: https://www.youtube.com/channel/UCjNZDC-ANZ23b6Qakv_1Yog
    title: YOUTUBE
    image_path: /assets/images/icon/youtube.png
    alt: "Youtube link"
  - url: https://assetstore.unity.com/publishers/36858
    title: ASSET STORE
    image_path: /assets/images/icon/unity.png
    alt: "Unity asset store link"
  - url: mailto:onecoin.studios@gmail.com
    title: EMAIL
    image_path: /assets/images/icon/email.png
    alt: "Emaiil link"
---

{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
  {% for post in collection.docs %}
    {% unless collection.output == false or collection.label == "posts" %}
      {% include archive-single.html %}
    {% endunless %}
  {% endfor %}
{% endfor %}

<a class="card" style="width: 18rem" href="https://www.youtube.com/channel/UCjNZDC-ANZ23b6Qakv_1Yog">
  <img src="/assets/images/icon/youtube.png" class="card-img-top" alt="Youtube">
</a>

<a class="card" style="width: 18rem" href="https://assetstore.unity.com/publishers/36858">
  <img src="/assets/images/icon/unity.png" class="card-img-top" alt="Unity">
</a>

<a class="card" style="width: 18rem" href="mailto:onecoin.studios@gmail.com">
  <img src="/assets/images/icon/email.png" class="card-img-top" alt="EMail">
</a>