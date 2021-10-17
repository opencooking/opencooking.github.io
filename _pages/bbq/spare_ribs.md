---
layout: page
title: Spare Ribs
permalink: /bbq/spare_ribs/
parent: BBQ
---
{% assign recipe = site.data.bbq.spareribs_321 %}

{% if recipe.Photo -%}
{% include gallery_style.liquid %}
<ul class="image-gallery">
    {% for pic in recipe.Photo %}
        <li><a href="/assets/images/recipes/{{ pic }}" title="" class="lightbox-image gallery"><img src="/assets/images/recipes/{{ pic }}" alt="" title=""><span></span></a></li>
    {% endfor %}
</ul>
{% endif -%}

# {{ recipe.Name }}
:exclamation:Zuerst herstellen: [BBQ Sauce Süss](/bbq/bbq_sauce_suess/):exclamation:
## Zutaten
{% for ingredient in recipe.Ingredients.Rub -%}
- {{ ingredient }}
{% endfor %}

## Rezept
{% for worksteps in recipe.Worksteps.Rub -%}
1. {{ worksteps }}
{% endfor %}