# mastering-markdown

Follow up repo of the Wes Bos course Mastering Markdown.

## Contents

- [mastering-markdown](#mastering-markdown)
  - [Contents](#contents)
  - [Paragraphs and text decoration](#paragraphs-and-text-decoration)
  - [Links](#links)
  - [Images](#images)
  - [Lists](#lists)
  - [Horizontal rules and block qoutes](#horizontal-rules-and-block-qoutes)
  - [Code blocks](#code-blocks)
  - [Tables](#tables)
  - [Check boxes](#check-boxes)

## Paragraphs and text decoration

This is *italic text*. This is also _italic text_.

This is **bold text**. This is also __bold text__.

This is ~~cross-out text~~.

## Links

Plain links look like this: <https://example.com>.

You can also add links to plain text, like [this](https://example.com).

Additionaly, you can add a hover description, like [this](https://example.com "some description"). Otherwise, the link is the description.

If links are long, or you want them organized all in one place, you can use ids, like [this][1]. Then, anywhere in the document (look at the end of this document), you define the link (it doesn't get rendered). This lets you reuse links.

## Images

They work like links. The syntax is ![alternate text (may be empty)](url or path).

They also can use the syntax with ids: ![alt text][2].

It's possible to set one image with a link to maybe a larger version of it, like this: [![alt text](url)](https://example.com).

It's also possible ot use HTML syntax [<img src="url" width="500" height="500" alt="alt text">](url) and CSS syntax

<style>
    img {
        width: 200px;
    }
</style>

## Lists

Unordered list (either *, + or -)

* first item
* second item

Ordered list

1. first item
   *. first sub item
        This is inline text for the first sub item.
      1. first sub sub item
   *. second sub item
2. second item

    This is a paragraph for the second item.

    This is a second paragraph for the second item.

Notice that numbered lists may have all it's items as 1, but they are redered incrementally.

1. first item
1. second item
1. third item

## Horizontal rules and block qoutes

The followin is a horizontal rule
***

> This is a block quote. - Anonymous

or

> This is a block quote.
>  
> \- **Anonymous**

## Code blocks

This is a code block:

```javascript
let x = 2;
const y = 'c';
```

This is inline code `let x = 0;`.

And this is diff syntax:

```diff
let x = 0;
- const y = 1;
+ const y = 0;
```

## Tables

|First column|Second column|Third column|
|:-----------|:-----------:|-----------:|
|abc|123|xxx|
|def|456|xxx|

## Check boxes

* [ ] first item
* [x] second item
* [ ] third item

[1]: https:example.com "some description"
[2]: https:example.com
