# The Markdown Guide

A simple and practical cheat sheet for GitHub Flavored Markdown (GFM), incorporating all the main features. It is intended to be used as both a showcase and a reference. 

For more information, visit [John Gruber's original specification](https://github.com) or the [GFM Getting Started Guide](https://docs.github.com/en/get-started/writing-on-github).





### Contents

- [Headings](#headings)
- [Emphasis](#emphasis)
- [Links](#links)
- [Images](#images)
- [Lists](#lists)
- [Blockquotes](#blockquotes)
- [Horizontal Rules](#horizontal-rules)
- [Raw HTML](#raw-html)
- [Code](#code)
- [Footnotes](#footnotes)
- [Tables](#tables)
- [Line Breaks](#line-breaks)
- [Videos](#videos)
- [TeX](#tex)





<h3 id="headings">Headings</h3>

```md
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```





<h3 id="emphasis">Emphasis</h3>

#### Italic

```md
*I'm italic*
_Same here_   
```

#### Bold

```md
**Bold here**
__Me too__   
```

#### Strikethrough

```md
~~Pineapple belongs on pizza~~
```

#### Combinations

```md
Feel free to try out the ~~**_combinations_**~~  
```





<h3 id="links">Links</h3>

#### Inline Links

```md 
[Google](https://www.google.com)
[With title](https://www.google.com "Title")
```

#### Reference Links

```md
[Example][reference]
Use numbers to reference links like [1]
Alternatively, simply use the [reference] for direct links
```

```md
[reference]: https://www.example.com   
[1]: https://www.example.com  
````

#### Relative Links

```md
[Link to the repository's license file](./LICENSE)
```

#### URLs

```md
http://www.example.com or <http://www.example.com> for direct links.
Sometimes, example.com works too (this behavior may differ depending on the renderer, such as GFM)
```





<h3 id="images">Images</h3>

#### Inline Images
```md
![Alt text](https://placehold.co/690x690/000000/FFFFFF.png?text=Cool+Text
```

#### Reference Images 

```md
![Alt text][placeholder-image]
```

```md
[placeholder-image]: https://placehold.co/690x690/000000/FFFFFF.png?text=Cool+Text
```

#### Relative Images

```md
![Alt text]["./imagineigotanimageherecuzigotnone.jpg"]
```





<h3 id="lists">Lists</h3>

> [!NOTE]
> An interpunct ("·") has been used to convey the concept of a space (" ") in some examples to ensure clarity

#### Unordered Lists

```md
* Asterisks  
- Minuses  
+ Pluses
```

#### Ordered Lists

```md
1. Item one
2. Item two
3. Item three
```

#### Nested Lists

```md
1. Item one
···2. Item two
······- Item three

- Item four
···- Item five
······6. Item six
```

#### Indented Paragraphs

```md
1. Item one
···You can add properly indented paragraphs within list items
···Notice the blank line above, and the leading spaces
```

```md
- Item two
···To create a line break without starting a new paragraph, add two trailing spaces··  
···This line is separate but still part of the same paragraph
```





<h3 id="blockquotes">Blockquotes</h3>

> [!NOTE]
> Blockquote styling is not part of the original Markdown spec. However, they're supported in **GitHub Flavored Markdown (GFM)**

```md
> This is a simple blockquote
> This is the second line
>> This is a nested blockquote
```

```md
> [!NOTE]
> This is a styled blockquote, a note

> [!TIP]
> This is a really cool tip

> [!IMPORTANT]
> This is a VERY important piece of text

> [!CAUTION]
> Hey, be cautious

> [!WARNING]
> This is a warning
```





<h3 id="horizontal-rules">Horizontal Rules</h1>

```md
Any
***
Three
---
Of
___
These
```





<h3 id="raw-html">Raw HTML</h1>

```html
<div>
  <p>Raw HTML works quite nicely in Markdown</p>
  <p>However **markdown** does __not__ work inside HTML</p>
  <p>Use <b>HTML</b> tags <i>instead</i></p>
</div>
```





<h3 id="code">Code</h1>

#### Inline Code

```md
This is some `very` cool `inline code`
```

#### Fenced Code Blocks

````md
```javascript
const variable = "My very cool variable"
console.log(variable)
```

```
Mo language is specified here, so no syntax highlighting (varies based on renderer). But hey, let's still add a <em>tag</em> because why not
```
````





<h3 id="footnotes">Footnotes</h1>

> [!NOTE]
> Footnotes are not part of the original Markdown spec. However, they're supported in **GitHub Flavored Markdown (GFM)**

```md
Here’s a basic footnote[^1].

Footnotes can also span multiple lines[^2].  

You can even name your footnotes for better organization or clarity[^note].

[^1]: This is the source or reference for the note
[^2]: To add multiple lines, simply start each new line with 2 spaces
    This makes it easy to create footnotes with more detailed information
[^note]: Named footnotes, like this one, will still display with numbers, but they offer easier identification and linking
    Notice the 4-space indentation for the new lines, which is a different syntax option.
```





<h3 id="tables">Tables</h1>

> [!NOTE]  
> Tables are not part of the original Markdown spec. However, they're supported in **GitHub Flavored Markdown (GFM)**

```md
| Left      | Center    | Right     |
| :-------- | :-------: | --------: |
| Apple     | Banana    | $1.00     |
| Orange    | Melon     | $0.75     |
```

```md
Markdown | Not | Formatted
--- | --- | ---
*Renders* | `the` | **same**
1 | 2 | 3
```





<h3 id="line-breaks">Line Breaks</h3>

```md
This is the first line in the first paragraph
This is the second line in the same paragraph, separated by a single new line from the one above

This is the first line in the second paragraph, separated by two new lines from the previous line of the previous paragraph 
```





<h3 id="videos">Videos</h1>

Markdown does not support videos natively. However, you can use embed a link to a video like this.

```html
<a href="http://www.youtube.com/watch?feature=player_embedded&v=VIDEO_ID><img src="http://img.youtube.com/vi/VIDEO_ID/thumbnail.jpg" alt="Alt text" width="690" height="420" border="5"/></a>
```

You can also use Markdown to directly embed the links. Keep in mind that this does not preserve the size or border.

```md
[![Alt Text](http://img.youtube.com/vi/VIDEO_ID/thumbnail.jpg)](http://www.youtube.com/watch?v=VIDEO_ID)
```





<h3 id="tex">TeX</h1>

> [!NOTE]
> TeX math expressions are enclosed using dollar signs ($).

A full list of TeX math symbols is beyond the scope of this cheatsheet. For a more comprehensive reference, check out [CodeCogs](https://codecogs.com/), where you can effectively experiment with equations. 

Still, here are some simple examples. 

```TeX
$E = mc^2$
```

```TeX
$\int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2}$
```

```TeX
$\int_0^\infty e^{-x^2} dx = \frac{\sqrt{\pi}}{2}$
```

