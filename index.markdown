---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      {{ post.excerpt }}
    </li>
  {% endfor %}
</ul>

<script src="/js/jquery.min.js"></script>

{% include comments.html element=".post-content" github_account="jhvanderschee/jekyllcodex" require_cookie_consent="true" %}

</body>
</html>
