# LB-2.0-Flex-Flora
A new 2.0-ready theme for Like Butter, based on Flex 'Flora' (by Out of the Sandbox)


Customisations
======================

File: `snippet/custom__dynamic-product-metafields.liquid`
File: `sections/product__main.liquid` 

Call the scripts to handle dynamic metafields

    {% comment %}LIke Butter customisation{% endcomment %}
    {% render 'custom__dynamic-product-metafields', product: product %}

Built by Satish Voddi (satish.voddi@storetasker.com), with thanks. 👏🏼

---


File: `sections/list-collections__main.liquid` 

Add collection description to the collections template output

    <span class="customisation__collection-description">
      {{ collection.description }}
    </span>

Exclude 'pre-order' collection from main collections output

    {% unless collection.handle == 'pre-order' %}
    {% endunless %}

---

File: `section/footer-classic.liquid.liquid`

Output template info

     <code class="test">Template name: {{template}}</code>

---

## Contact:

Jay Armstrong, Like Butter
cuts@likebutter.com.au
