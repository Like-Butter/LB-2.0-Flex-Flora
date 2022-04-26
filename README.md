# LB-2.0-Flex-Flora
A new 2.0-ready theme for Like Butter, based on Flex 'Flora' (by Out of the Sandbox)
======================

# Dynamic metafields on product templates

1. assets/utilies.js

    document.dispatchEvent(new CustomEvent('variant:change', {detail: {productEl, product, variant, state}}));

1. snippet/custom__dynamic-product-metafields.liquid
1. sections/product__main.liquid

    {% comment %}LIke Butter customisation{% endcomment %}
    {% render 'custom__dynamic-product-metafields', product: product %}

Built by Satish Voddi (satish.voddi@storetasker.com), with thanks. 👏🏼

---


`sections/list-collections__main.liquid` 

Add collection description to the collections template output

    <span class="customisation__collection-description">
      {{ collection.description }}
    </span>

Exclude 'pre-order' collection from main collections output

    {% unless collection.handle == 'pre-order' %}
    {% endunless %}


---

## Contact:

Jay Armstrong, Like Butter
cuts@likebutter.com.au
