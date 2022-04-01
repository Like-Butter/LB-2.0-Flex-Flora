# LB-2.0-Flex-Flora
A new 2.0-ready theme for Like Butter, based on Flex 'Flora' (by Out of the Sandbox)


Customisations
======================

File: `list-collections__main.liquid` 

Add collection description to the collections template output

    <span class="customisation__collection-description">
      {{ collection.description }}
    </span>

Exclude 'pre-order' collection from main collections output

    {% unless collection.handle == 'pre-order' %}
    {% endunless %}




## Contact:

Jay Armstrong, Like Butter
cuts@likebutter.com.au
