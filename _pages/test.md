---
title: Test
permalink: /test/
---


# This is Header 1
## This Header 2
### H3
#### H4
##### H5
###### H6?

'' block quote I think!

'just italics'

**this ought to be bold**

Give me [a link](https://www.google.com)

Content is written in [Markdown](https://learnxinyminutes.com/docs/markdown/).
Plain text format allows you to focus on your **content**.

<!--
You can use HTML elements in Markdown, such as the comment element, and they won't
be affected by a markdown parser. However, if you create an HTML element in your
markdown file, you cannot use markdown syntax within that element's contents.
-->

<!-- Pagination links -->
<nav class="pagination">
  {% if paginator.previous_page %}
    {% if paginator.previous_page == 1 %}
      <a href="/" class="previous">&laquo;</a>
    {% else %}
      <a href="/page" class="previous">&laquo;</a>
    {% endif %}
  {% endif %}
  {% if paginator.next_page %}
    <a href="/page" class="next ">&raquo;</a>
  {% endif %}
</nav>

{% for post in paginator.posts %}
  ... your post list HTML ...
{% endfor %}