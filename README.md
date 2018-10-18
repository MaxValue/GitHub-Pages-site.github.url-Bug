---
---
# GitHub-Pages-Bug
_test repository demonstrating the bug_

This site shows and tests the presence of a bug in GitHub Pages

I noticed that the Jekyll version used GitHub Pages is malconfigured in a way
that the variable `site.github.url` does not point to the web location of the site itself
but to a non-existent page on GitHub. This page demonstrates this
and also verifies the presence of this bug.

### Dynamic Link
###### {{ site.github.url }}

### Hardcoded Link
###### https://maxvalue.github.io/GitHub-Pages-site.github.url-Bug/

The above 2 links should be exactly the same.

## Status:
{% if site.github.url == "https://maxvalue.github.io/GitHub-Pages-site.github.url-Bug/" %}
&#x2B55; The bug has been fixed!
{% else %}
&#x274C; This bug is present.
{% endif %}

## Further Infos
This bug has been noticed on project AND user pages.
