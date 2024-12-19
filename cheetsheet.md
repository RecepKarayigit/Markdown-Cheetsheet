# Extended Markdown Features

This README.md file demonstrates various features of Markdown with a more extensive explanation, examples, and notes. Some of these features are GitHub-specific, while others are standard Markdown syntax. Let's explore each feature, along with any relevant usage considerations or enhancements.


## 1. Line Breaks in Markdown
In Markdown, text is displayed as a continuous block of text without automatic line breaks, unless you explicitly tell it to break the line.

To create a line break in Markdown, you need to either:

Use HTML <br> tags: This works on most Markdown platforms, including GitHub.
Add two spaces at the end of the line: This tells Markdown to create a line break.
Without these methods, Markdown will treat the text as part of the same paragraph, and it won't break lines even if you press "Enter."

<u>**Markdown Syntax:**</u>
```markdown
This is a paragraph.
This is another sentence in the same paragraph.

This is a paragraph.<br>And this is the second line.

This is a paragraph.  
And this is the second line.
```
<u>**Rendered Result:**</u>

This is a paragraph.
This is another sentence in the same paragraph.

This is a paragraph.<br>And this is the second line.

This is a paragraph.  
And this is the second line.

> **Note**: Markdown might automatically combine lines if only one space is added. Use two spaces at the end of the line to force a break.


## 2. Headings

Markdown allows you to create headings of different levels by using `#` symbols. More `#` symbols mean a smaller heading level. 

<u>**Markdown Syntax:**</u>
```markdown
# H1
## H2
### H3
#### H4
##### H5
###### H6
```
<u>**Rendered Result:**</u>
# H1
## H2
### H3
#### H4
##### H5
###### H6

> **Note**: Always ensure that there is a space between the `#` symbols and the heading text.

---

## 3. Emphasis

You can emphasize text using `*` or `_` for italics and `**` or `__` for bold. You can also use `~~` for strikethrough.

<u>**Markdown Syntax:**</u>
```markdown
*Italic*
_Italic_
**Bold**
__Bold__
~~Strikethrough~~
```

<u>**Rendered Result:**</u>
*Italic*  
_Italic_  
**Bold**  
__Bold__  
~~Strikethrough~~

> **Note**: Be cautious of using too many styles at once, as it might make the content hard to read. For example, avoid **_bold and italic_** for large sections of text.

---

## 4. Ordered List

Markdown supports ordered lists, where each item is numbered automatically. You can also create nested ordered lists.

<u>**Markdown Syntax:**</u>
```markdown
1. First item
2. Second item
   1. Subitem
   2. Another subitem
3. Third item
***
71. First item
1. Second item
   1. Subitem
   1. Another subitem
1. Third item
```

<u>**Rendered Result:**</u>
1. First item
2. Second item
   1. Subitem
   2. Another subitem
3. Third item
***
71. First item
1. Second item
   1. Subitem
   1. Another subitem
1. Third item

> **Note**: You can use any number for the list (e.g., `1.` or `2.`), Markdown will automatically render them in order.

---

## 5. Unordered List

Unordered lists are created using `-`, `*`, or `+` symbols.

<u>**Markdown Syntax:**</u>
```markdown
- Item 1
  - Subitem A
  - Subitem B
- Item 2
  - Subitem C

* Item 3
  * Subitem A
  * Subitem B
* Item 4
  * Subitem C

+ Item 5
  + Subitem A
  + Subitem B
+ Item 6
  + Subitem C
```

<u>**Rendered Result:**</u>
- Item 1
  - Subitem A
  - Subitem B
- Item 2
  - Subitem C

* Item 3
  * Subitem A
  * Subitem B
* Item 4
  * Subitem C

+ Item 5
  + Subitem A
  + Subitem B
+ Item 6
  + Subitem C 

> **Note**: While all three symbols (`-`, `*`, `+`) are supported, it’s a good practice to choose one and stick with it for consistency.

---

## 6. Links

Markdown allows you to link to websites or other resources. Links can be inline or reference-style.

<u>**Markdown Syntax:**</u>
```markdown
[GitHub](https://github.com)
[GitHub][1]
[1]: https://github.com
```

<u>**Rendered Result:**</u>
[GitHub](https://github.com)  
[GitHub][1]  
[1]: https://github.com

> **Note**: Use reference links when the URL appears multiple times in the document to improve readability and maintainability.

---

## 7. Images

Images are inserted in Markdown using an exclamation mark `!`, followed by the alt text in square brackets and the image URL in parentheses.

<u>**Markdown Syntax:**</u>
```markdown
![GitHub Logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)
```

<u>**Rendered Result:**</u>
![GitHub Logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)

> **Note**: Image dimensions are not supported directly in standard Markdown. If you need to resize an image, you might need to use HTML within Markdown.

<u>**Markdown Syntax:**</u>
```markdown
<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="200" height="200" />
```
<u>**Rendered Result:**</u>
<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" width="200" height="200" />

---

## 8. Inline Code

Inline code is enclosed within backticks (`).

<u>**Markdown Syntax:**</u>
```markdown
Use the `print()` function in Python.
```

<u>**Rendered Result:**</u>
Use the `print()` function in Python.

> **Note**: Be careful with using backticks in plain text that is not code, as it might cause confusion in the context of documentation.

---

## 9. Code Block

Code blocks can be created with triple backticks (```), followed by the language name for syntax highlighting.

<u>**Markdown Syntax:**</u>
```markdown
```python
def hello():
    print("Hello, World!")
```
```

<u>**Rendered Result:**</u>
```python
def hello():
    print("Hello, World!")
```

> **Note**: Always specify the language for better syntax highlighting (e.g., `python`, `javascript`).

---

## 10. Blockquotes

Blockquotes are created using the `>` symbol.

<u>**Markdown Syntax:**</u>
```markdown
> "The only limit to our realization of tomorrow is our doubts of today."  
> - Franklin D. Roosevelt
```

<u>**Rendered Result:**</u>
> "The only limit to our realization of tomorrow is our doubts of today."  
> - Franklin D. Roosevelt

  
> **Note**: Blockquotes can be nested by adding extra `>` symbols, for example, `>>` for a nested quote.

<u>**Markdown Syntax:**</u>
```markdown
> This is a blockquote.
> 
> > This is a nested blockquote.
> > 
> > > This is a double-nested blockquote.
```

<u>**Rendered Result:**</u>
> This is a blockquote.
> 
> > This is a nested blockquote.
> > 
> > > This is a double-nested blockquote.
---

## 11. Horizontal Rule

A horizontal rule is a line that separates sections of content and is created using three or more hyphens (`---`), asterisks (`***`), or underscores (`___`).

<u>**Markdown Syntax:**</u>
```markdown
---
***
___
```

<u>**Rendered Result:**</u>

---
***
___

> **Note**: A horizontal rule can also be styled using `*` or `_`, depending on your preference.
<u>**Markdown Syntax:**</u>
```markdown
*__________*
**__________**
~~__________~~
```
<u>**Rendered Result:**</u>

*__________*
**__________**
~~__________~~

---

## 12. Tables

Tables are created using pipes (`|`) and dashes (`-`) for the header and separator row.

<u>**Markdown Syntax:**</u>
```markdown
| Header 1 | Header 2 |
|----------|----------|
| Data 1   | Data 2   |
```

<u>**Rendered Result:**</u>
| Header 1 | Header 2 |
|----------|----------|
| Data 1   | Data 2   |

> **Note**: In Markdown, tables support text alignment using colons ( : ) in the separator row: 
>
> :--- aligns text to the left.
> :---: centers the text.
> ---: aligns text to the right. 
>
> This method works in most Markdown parsers, including GitHub. However, keep in mind that the column width is determined by the content, and there is no direct support for controlling column size. Ensure alignment is properly applied by placing colons correctly in the separator row.
>
> <u>**Markdown Syntax:**</u>
> ```markdown
> | Left Align   | Center Align   | Right Align   |
> |:-------------|:--------------:|--------------:|
> | Item 1       | Item 2         | Item 3        |
> | Item 4       | Item 5         | Item 6        |
> ```
> <u>**Rendered Result:**</u>
> | Left Align   | Center Align   | Right Align   |
> |:-------------|:--------------:|--------------:|
> | Item 1       | Item 2         | Item 3        |
> | Item 4       | Item 5         | Item 6        |


---

## 13. Task Lists

You can create task lists with checkboxes by using `- [ ]` for an unchecked item and `- [x]` for a checked item.

<u>**Markdown Syntax:**</u>
```markdown
- [x] Task 1
- [ ] Task 2
```

<u>**Rendered Result:**</u>
- [x] Task 1  
- [ ] Task 2

> **Note**: Task lists are particularly useful for tracking progress in a project. GitHub supports task lists in issues and pull requests.

---

## 14. Escape Characters

To escape special characters (like `*`, `#`, etc.), use a backslash (`\`) before the character.

<u>**Markdown Syntax:**</u>
```markdown
\*This is not italic\*
```

<u>**Rendered Result:**</u>
\*This is not italic\*

> **Note**: Be mindful when using escape characters, especially in situations where you want to include Markdown symbols literally, rather than applying their formatting.

---

## 15. Syntax Highlighting

You can highlight code blocks with syntax highlighting by specifying the language after the triple backticks.

<u>**Markdown Syntax:**</u>
```markdown
```python
def add(a, b):
    return a + b
```
```

<u>**Rendered Result:**</u>
```python
def add(a, b):
    return a + b
```

> **Note**: Ensure the language name is correctly spelled to apply the right syntax highlighting.

---

## 16. Emojis

GitHub supports a wide range of emojis, which can be added using their shortcodes (e.g., `:smile:`).

<u>**Markdown Syntax:**</u>
```markdown
:smile: :+1: :tada:
```

<u>**Rendered Result:**</u>
:smile: :+1: :tada:

> **Note**: Emojis are widely supported on GitHub but may not render properly on all Markdown renderers outside of GitHub. https://gist.github.com/rxaviers/7360908 repository contains a collection of emoji shortcodes that you can use in your Markdown files to enhance visual appeal or convey emotions more effectively. Simply copy the emoji shortcodes from the list and insert them into your document.
---

## 17. Mentions

GitHub supports mentions of users, teams, and repositories using the `@` symbol.

<u>**Markdown Syntax:**</u>
```markdown
@username
```

<u>**Rendered Result:**</u>
@username

> **Note**: Mentions will trigger notifications for the mentioned user or team only on GitHub.

---

## 18. Issues/PR Links

You can link to issues or pull requests by using `#` followed by the issue or PR number.

<u>**Markdown Syntax:**</u>
```markdown
#123
```

<u>**Rendered Result:**</u>
#123

> **Note**: This works on GitHub to automatically link to the issue or PR.

---

## 19. Reference Links

You can define links separately and reference them later in the document.

<u>**Markdown Syntax:**</u>
```markdown
[GitHub][1]

[1]: https://github.com
```

<u>**Rendered Result:**</u>
[GitHub][1]  
[1]: https://github.com

> **Note**: Reference links help keep Markdown documents neat and maintainable, especially for frequently used URLs.

---

## 20. HTML Support

Markdown supports HTML elements, which can be useful for styling and other complex structures.

<u>**Markdown Syntax:**</u>
```markdown
<b>Bold Text</b>
```

<u>**Rendered Result:**</u>
**Bold Text**

> **Note**: Be cautious with HTML as it may break the simplicity of Markdown. It's best used sparingly.

---

## 21. Footnotes

GitHub does not natively support footnotes in Markdown, but it can be done using HTML for more advanced documentation needs.

<u>**Markdown Syntax:**</u>
```markdown
Here is a reference[^1].
[^1]: This is the footnote.
```

<u>**Rendered Result:**</u>
Here is a reference[^1].  
[^1]: This is the footnote.

> **Note**: GitHub does not render footnotes by default, and you will need to use HTML tags for creating custom footnotes.

---

## 22. Keyboard Keys

You can denote keyboard keys using `<kbd>` tags.

<u>**Markdown Syntax:**</u>
```markdown
<kbd>Ctrl</kbd>+<kbd>C</kbd>
```

<u>**Rendered Result:**</u>
<kbd>Ctrl</kbd>+<kbd>C</kbd>

> **Note**: This feature is mostly supported on GitHub and may not render consistently across all Markdown renderers.

---

## 23. Collapsible Sections

GitHub supports collapsible sections, useful for organizing long documents.

<u>**Markdown Syntax:**</u>
```markdown
<details><summary>Click to expand</summary>
This content is hidden until the user clicks to reveal it.
</details>
```

<u>**Rendered Result:**</u>
<details><summary>Click to expand</summary>
This content is hidden until the user clicks to reveal it.
</details>

> **Note**: Collapsible sections are supported on GitHub but may not work on all Markdown platforms.

---

For more detailed information, you can refer to the [GitHub Markdown Guide](https://guides.github.com/features/mastering-markdown/).
