# README Reference

Here, I collate Github Flavor Markdown syntax for quick reference.

## Format

- Must have:
  - Project title
  - Project description
  - Installation & usage
  - Technologies
  - Process
  - Licence
- Should have:
  - Screenshots/Images
  - Wins & Challenges
- Could have:
  - Badges
  - Contribution guide
  - Code snippets
  - Bugs
  - Future features

## Useful Tools

- [Markdown Guide](https://guides.github.com/features/mastering-markdown/)
- [Badges](https://medium.com/better-programming/add-badges-to-a-github-repository-716d2988dc6a)

A bigger list of tools (that probably negates the need for this page) can be found at [github.com/writekit/awesome-markdown](https://github.com/writekit/awesome-markdown).

### Tools

### Editors

- [StackEdit](https://stackedit.io): In-browser MD document editor
- [Minimalist Online Markdown Editor](http://markdown.pioul.fr/)
- [Mou](http://25.io/mou/): macOS editor
- [Haroopad](http://pad.haroopress.com/user.html): Cross-platform editor

### Libraries

#### JavaScript

- [Marked](https://github.com/chjj/marked)
- [Remarkable](https://github.com/jonschlinkert/remarkable)
- [PageDown](https://code.google.com/p/pagedown/) (and [PageDown Extra](https://github.com/jmcmanus/pagedown-extra))
- [markdown-it](https://github.com/markdown-it/markdown-it)
- [Gitdown](https://github.com/gajus/gitdown): GitHub markdown preprocessor
- [reMarked.js](https://github.com/leeoniya/reMarked.js): HTML-to-Markdown processor
- [Kramed](https://github.com/GitbookIO/kramed): Fork of Marked

# Reference

This is intended as a quick reference and showcase. For more complete info, see [John Gruber's original spec](http://daringfireball.net/projects/markdown/) and the [Github-flavored Markdown info page](http://github.github.com/github-flavored-markdown/).

## Emphasis

- Emphasis, aka italics, with _asterisks_ or _underscores_.
- Strong emphasis, aka bold, with **asterisks** or **underscores**.
- Combined emphasis with **asterisks and _underscores_**.
- Strikethrough uses two tildes. ~~Scratch this.~~

## Lists

1. First ordered list item
2. Another item

- Unordered sub-list.

1. Actual numbers don't matter, just that it's a number
1. Ordered sub-list
1. And another item.

   You can have properly indented paragraphs within list items. Notice the blank line above, and the leading spaces (at least one, but we'll use three here to also align the raw Markdown).

   To have a line break without a paragraph, you will need to use two trailing spaces.  
   Note that this line is separate, but within the same paragraph.  
   (This is contrary to the typical GFM line break behaviour, where trailing spaces are not required.)

- Unordered list can use asterisks

* Or minuses

- Or pluses

## Links

There are two ways to create links.

- [I'm an inline-style link](https://www.google.com)
- [I'm an inline-style link with title](https://www.google.com "Google's Homepage")
- [I'm a reference-style link][Arbitrary case-insensitive reference text]
- [I'm a relative reference to a repository file](../blob/master/LICENSE)
- [You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links.
http://www.example.com or <http://www.example.com> and sometimes
example.com (but not on Github, for example).

Some text to show that the reference links can follow later.

[arbitrary case-insensitive reference text]: https://www.mozilla.org
[1]: http://slashdot.org
[link text itself]: http://www.reddit.com

## Images

Hover to see the title text

Inline-style:
![alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/f/fa/718smiley.png/90px-718smiley.png "Logo Title Text 1")

Reference-style:
![alt text][logo]

[logo]: https://upload.wikimedia.org/wikipedia/commons/thumb/f/fa/718smiley.png/90px-718smiley.png "Logo Title Text 2"

## Code and Syntax Highlighting

Code blocks are part of the Markdown spec, but syntax highlighting isn't. However, many renderers -- like Github's and _Markdown Here_ -- support syntax highlighting. Which languages are supported and how those language names should be written will vary from renderer to renderer. _Markdown Here_ supports highlighting for dozens of languages (and not-really-languages, like diffs and HTTP headers); to see the complete list, and how to write the language names, see the [highlight.js demo page](http://softwaremaniacs.org/media/soft/highlight/test.html).

```no-highlight
Inline `code` has `back-ticks around` it.
```

Inline `code` has `back-ticks around` it.

Blocks of code are either fenced by lines with three back-ticks <code>```</code>, or are indented with four spaces. I recommend only using the fenced code blocks -- they're easier and only they support syntax highlighting.

<pre lang="no-highlight"><code>```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
 
```python
s = "Python syntax highlighting"
print s
```
 
```
No language indicated, so no syntax highlighting. 
But let's throw in a &lt;b&gt;tag&lt;/b&gt;.
```
</code></pre>

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

```python
s = "Python syntax highlighting"
print s
```

```
No language indicated, so no syntax highlighting in Markdown Here (varies on Github).
But let's throw in a <b>tag</b>.
```

## Tables

Tables aren't part of the core Markdown spec, but they are part of GFM and _Markdown Here_ supports them. They are an easy way of adding tables to your email -- a task that would otherwise require copy-pasting from another application.

```no-highlight
Colons can be used to align columns.

| Tables        | Are           | Cool  |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |

There must be at least 3 dashes separating each header cell.
The outer pipes (|) are optional, and you don't need to make the
raw Markdown line up prettily. You can also use inline Markdown.

Markdown | Less | Pretty
--- | --- | ---
*Still* | `renders` | **nicely**
1 | 2 | 3
```

Colons can be used to align columns.

| Tables        |      Are      |  Cool |
| ------------- | :-----------: | ----: |
| col 3 is      | right-aligned | $1600 |
| col 2 is      |   centered    |   $12 |
| zebra stripes |   are neat    |    $1 |

There must be at least 3 dashes separating each header cell. The outer pipes (|) are optional, and you don't need to make the raw Markdown line up prettily. You can also use inline Markdown.

| Markdown | Less      | Pretty     |
| -------- | --------- | ---------- |
| _Still_  | `renders` | **nicely** |
| 1        | 2         | 3          |

## Blockquotes

> Blockquotes are very handy in email to emulate reply text.
> This line is part of the same quote.

Quote break.

> This is a very long line that will still be quoted properly when it wraps. Oh boy let's keep writing to make sure this is long enough to actually wrap for everyone. Oh, you can _put_ **Markdown** into a blockquote.

## Inline HTML

You can also use raw HTML in your Markdown, and it'll mostly work pretty well.

```no-highlight
<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>
```

<dl>
  <dt>Definition list</dt>
  <dd>Is something people use sometimes.</dd>

  <dt>Markdown in HTML</dt>
  <dd>Does *not* work **very** well. Use HTML <em>tags</em>.</dd>
</dl>

## Horizontal Rule

```
Three or more...

---

Hyphens

***

Asterisks

___

Underscores
```

Three or more...

---

Hyphens

---

Asterisks

---

Underscores

## Line Breaks

My basic recommendation for learning how line breaks work is to experiment and discover -- hit &lt;Enter&gt; once (i.e., insert one newline), then hit it twice (i.e., insert two newlines), see what happens. You'll soon learn to get what you want. "Markdown Toggle" is your friend.

Here are some things to try out:

```
Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a *separate paragraph*.

This line is also a separate paragraph, but...
This line is only separated by a single newline, so it's a separate line in the *same paragraph*.
```

Here's a line for us to start with.

This line is separated from the one above by two newlines, so it will be a _separate paragraph_.

This line is also begins a separate paragraph, but...  
This line is only separated by a single newline, so it's a separate line in the _same paragraph_.

(Technical note: _Markdown Here_ uses GFM line breaks, so there's no need to use MD's two-space line breaks.)

## YouTube Videos

They can't be added directly but you can add an image with a link to the video like this:

```html
<a
  href="http://www.youtube.com/watch?feature=player_embedded&v=YOUTUBE_VIDEO_ID_HERE
"
  target="_blank"
  ><img
    src="http://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg"
    alt="IMAGE ALT TEXT HERE"
    width="240"
    height="180"
    border="10"
/></a>
```

Or, in pure Markdown, but losing the image sizing and border:

```md
[![Deploying a Distributed Ray Python Server with Kubernetes, EKS & KubeRay to serve our own LLM](https://img.youtube.com/vi/GEuM9rXtmkk/0.jpg)](https://www.youtube.com/watch?v=GEuM9rXtmkk)
```

[![Deploying a Distributed Ray Python Server with Kubernetes, EKS & KubeRay to serve our own LLM](https://img.youtube.com/vi/GEuM9rXtmkk/0.jpg)](https://www.youtube.com/watch?v=GEuM9rXtmkk)

## Using emoji

GitHub supports emoji!

To see a list of every image we support, check out the [Emoji Cheat Sheet](http://www.emoji-cheat-sheet.com/).

## How to add a collapsible section in markdown.

````md
<details>
  <summary>Click me</summary>
  
  ### Heading
  1. Foo
  2. Bar
     * Baz
     * Qux

### Some Code

```js
function logSomething(something) {
  console.log("Something", something);
}
```

</details>
````

## Example

<details>
    <summary>Click me</summary>

### Heading

1. Foo
2. Bar
   - Baz
   - Qux

### Some Code

```js
function logSomething(something) {
  console.log("Something", something);
}
```

</details>

## Rules

1. Have an **empty line** after the `</summary>` tag or markdown/code blocks will not render.
1. Have an **empty line** after each `</details>` tag if you have multiple collapsible sections.

## TeX Mathematical Formulae

A full description of TeX math symbols is beyond the scope of this cheatsheet. Here's a [good reference](https://en.wikibooks.org/wiki/LaTeX/Mathematics), and you can try stuff out on [CodeCogs](https://www.codecogs.com/latex/eqneditor.php). You can also play with formulae in the Markdown Here options page.

Here are some examples to try out:

```
$-b \pm \sqrt{b^2 - 4ac} \over 2a$
$x = a_0 + \frac{1}{a_1 + \frac{1}{a_2 + \frac{1}{a_3 + a_4}}}$
$\forall x \in X, \quad \exists y \leq \epsilon$
```

The beginning and ending dollar signs (`$`) are the delimiters for the TeX markup.

$\forall x \in X, \quad \exists y \leq \epsilon$

## Add Caption to Images

Use table for this. It works fine.

<!-- prettier-ignore -->
```md
| ![space-1.jpg](https://i.imgur.com/1qyuqBp.png) | 
|:--:| 
| *Caption* |
```

<!-- prettier-ignore -->
| ![space-1.jpg](https://i.imgur.com/1qyuqBp.png) | 
|:--:| 
| *Caption* |

## Alerts

[Alerts](https://github.com/orgs/community/discussions/16925) are an extension of Markdown used to emphasize critical information. On GitHub, they are displayed with distinctive colors and icons to indicate the importance of the content.

> [!NOTE]  
> Highlights information that users should take into account, even when skimming.

> [!TIP]
> Optional information to help a user be more successful.

> [!IMPORTANT]  
> Crucial information necessary for users to succeed.

> [!WARNING]  
> Critical content demanding immediate user attention due to potential risks.

> [!CAUTION]
> Negative potential consequences of an action.

## Footnotes

Footnotes aren't part of the core Markdown spec, but they [supported by GFM](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#footnotes).

```no-highlight
Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

You can also use words, to fit your writing style more closely[^note].

[^1]: My reference.
[^2]: Every new line should be prefixed with 2 spaces.
  This allows you to have a footnote with multiple lines.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.
    This footnote also has been made with a different syntax using 4 spaces for new lines.
```

Renders to:

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].

You can also use words, to fit your writing style more closely[^note].

[^1]: My reference.
[^2]:
    Every new line should be prefixed with 2 spaces.
    This allows you to have a footnote with multiple lines.

[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.
    This footnote also has been made with a different syntax using 4 spaces for new lines.
