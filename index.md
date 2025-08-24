# _config.yml (Configuration for Jekyll)
theme: minima
title: My Blog & Documentation
description: A simple blog and documentation site with payment options
baseurl: ""
url: "https://username.github.io"
header_pages:
  - about.md
  - payment.md
  - blog.md

# Create directory structure and files
---
# index.md (Homepage)
---
# Welcome to My Blog & Docs

This is a simple blog and documentation site built with Jekyll. Check out the [Blog](blog.md), [About](about.md), or [Payment](payment.md) pages.

## Latest Posts
{% for post in site.posts %}
  - [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%b %d, %Y" }}
{% endfor %}

---
# about.md (About Page)
---
# About This Site

This site serves as a blog and documentation hub. It’s built with Jekyll, hosted on GitHub Pages, and includes a payment option for support.

---
# payment.md (Payment Page with Image and Donation Form)
---
# Payment Options

Support this blog and documentation site! Below are the payment options, including a donation form.

![Payment Image](https://via.placeholder.com/300x200) <!-- Replace with your image URL -->

## Donation Form
<form action="https://www.paypal.com/donate" method="post" target="_top">
  <input type="hidden" name="hosted_button_id" value="YOUR_PAYPAL_BUTTON_ID" /> <!-- Replace with PayPal button ID -->
  <input type="image" src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif" border="0" name="submit" title="PayPal - The safer, easier way to pay online!" alt="Donate with PayPal button" />
</form>

## Other Payment Methods
- **PayPal**: Send to https://buymeacoffee.com/aanandjha
- **Buy Me a Coffee**: [Support via Buy Me a Coffee](https://buymeacoffee.com/aanandjha)
- **Crypto**: BTC address: `bc1qwvnfan4082zk3gu5g8ym0alkg3zevqm6v5dk8u`

---
# blog.md (Blog Listing Page)
---
# Blog Posts

All posts are listed below:

{% for post in site.posts %}
  - [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%b %d, %Y" }}
{% endfor %}

---
# _posts/2025-08-24-first-post.md (Sample Blog Post)
---
layout: post
title: First Blog Post
date: 2025-08-24
---

This is the first blog post. Write your content here in Markdown. You can add more posts by creating new files in the `_posts` directory with the format `YYYY-MM-DD-title.md`.

---
# _posts/2025-08-24-second-post.md (Sample Blog Post)
---
layout: post
title: Documentation Example
date: 2025-08-24
---

This is a sample documentation post. Use this format for tutorials or guides. Markdown makes it easy to format code, lists, and more.

```bash
# Example code block
echo "Hello, Jekyll!"
