# LB-2.0-Flex-Flora

A new 2.0-ready theme for Like Butter, based on Flex 'Flora' (by Out of the Sandbox)




# Dynamic metafields on product templates
Built by Satish Voddi (satish.voddi@storetasker.com), with thanks. 👏🏼

### assets/utilies.js

    document.dispatchEvent(new CustomEvent('variant:change', {detail: {productEl, product, variant, state}}));

### sections/product__main.liquid

    {% comment %}Like Butter customisation{% endcomment %}
    {% render 'product-dynamic-metafield-scripts', product: product %}

### snippets/product-dynamic-metafield-scripts.liquid

---

# Product template customisations

### snippets/product__form.liquid

Inject the 'lead times' metafield immediately below the product form block

---

# Collection template customisations

### sections/list-collections__main.liquid

Add collection description to the collections template output

    <span class="customisation__collection-description">
      {{ collection.description }}
    </span>

---

# Exclude collections

Exclude 'pre-order' collection from main collections output

    {% unless collection.handle == 'pre-order' %}
    {% endunless %}

---

# Inject metafields

{% render 'custom__designer' %} into snippets/products.liquid

{% render 'custom__lead-time' %} into snippets/products__form.liqiud

---

Contact: Jay Armstrong, Like Butter
cuts@likebutter.com.au
