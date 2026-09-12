---
title: Writing a New Post
author: cotes
date: 2019-08-08 14:10:00 +0800
categories: [Blogging, Tutorial]
tags: [writing]
render_with_liquid: false
---

This tutorial will guide you on how to write a post in the _Chirpy_ template.

## Naming and Path

Create a new file named `YYYY-MM-DD-TITLE.EXTENSION`{: .filepath} and put it in the `_posts`{: .filepath} of the root directory.

## Front Matter

Basically, you need to fill the Front Matter as below at the top of the post:

```yaml
---
title: TITLE
date: YYYY-MM-DD HH:MM:SS +/-TTTT
categories: [TOP_CATEGORY, SUB_CATEGORY]
tags: [TAG]     # TAG names should always be lowercase
---
```

> The posts' _layout_ has been set to `post` by default, so there is no need to add the variable _layout_ in the Front Matter block.
{: .prompt-tip }

### Categories and Tags

The `categories` of each post are designed to contain up to two elements, and the number of elements in `tags` can be zero to infinity.

## Table of Contents

By default, the Table of Contents (TOC) is displayed on the right panel of the post.

## Comments

The global setting for comments is defined by the `comments.provider` option in the `_config.yml`{: .filepath} file.

## Media

We refer to images, audio and video as media resources in _Chirpy_.

### Images

#### Caption

Add italics to the next line of an image, then it will become the caption:

```markdown
![img-description](/path/to/image)
_Image Caption_
```

#### Size

To prevent the page content layout from shifting when the image is loaded, we should set the width and height for each image.

```markdown
![Desktop View](/assets/img/sample/mockup.png){: width="700" height="400" }
```

## Pinned Posts

You can pin one or more posts to the top of the home page:

```yaml
---
pin: true
---
```

## Prompts

There are several types of prompts: `tip`, `info`, `warning`, and `danger`.

```md
> Example line for prompt.
{: .prompt-info }
```

## Learn More

For more knowledge about Jekyll posts, visit the Jekyll Docs: Posts.
