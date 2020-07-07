
# Usage 

Run with pandoc-eisvogel using the following:

```
pandoc blog_test-hugo_blog.md  -o post.pdf --from markdown --template eisvogel --listings
```

# Changes to post.md to make it work

* remove `{{< output> }}` and `{{</output>}}`, as it is unnecessary
* remove latex code blocks, as they are not interpretable
* metadata must change from:
+++
title = "title"

instead to:
---
title: "title"



# Changes to styling

* create appropriate header / title page
* fix tabular output, probably with .css
* allow for removal of code, when desired
* fix image for correct output directory
