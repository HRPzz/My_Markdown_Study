# Markdown Grammar

## 1. Headers

### 1-1. Use `#`: H1 to H6

```markdown
# Header 1
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6
```

# Header 1

## Header 2

### Header 3

#### Header 4

##### Header 5

###### Header 6

### 1-2. Use `===`: Same as H1

1. Write `Header Texts`
2. Write `===` on the next line

```markdown
Header 1
===
```

Header 1
===

### 1-3. Use `---`: Same as H2

1. Write `Header Texts`
2. Write `---` on the next line

```markdown
Header 2
---
```

Header 2
---

## 2. horizon: Use `***` or `---`

```markdown
* * *

***

*****

- - -

---
```

* * *

***

- - -

---

## 3. Line breaks

### 3-1. Use `Enter` at the end of the text

```markdown
Where the world builds software

Millions of developers and companies build, ship, and maintain their software on GitHub—the largest and most advanced development platform in the world.
```

Where the world builds software
Millions of developers and companies build, ship, and maintain their software on GitHub—the largest and most advanced development platform in the world.

### 3-2. Use `Spacebar 2` at the end of the text

```markdown
Where the world builds software  
Millions of developers and companies build, ship, and maintain their software on GitHub—the largest and most advanced development platform in the world.
```

Where the world builds software  
Millions of developers and companies build, ship, and maintain their software on GitHub—the largest and most advanced development platform in the world.

### 3-3. Use the `<br>` tag at the end of the text

```markdown
Where the world builds software<br>
Millions of developers and companies build, ship, and maintain their software on GitHub—the largest and most advanced development platform in the world.
```

Where the world builds software<br>
Millions of developers and companies build, ship, and maintain their software on GitHub—the largest and most advanced development platform in the world.

## 4. Emphasis

### 4-1. Italics: `_Text_`, `*Text*`

```markdown
_Text_

*Text*
```

_Text_

_Text_

### 4-2. Bold: `__Text__`, `**Text**`

```markdown
__Text__

**Text**
```

__Text__

__Text__

### 4-3. Italics and Bold: `__*Text*__`, `**_Text_**`

```markdown
__*Text*__

**_Text_**
```

___Text___

**_Text_**

## 5. Lists

### 5-1. Unordered Lists: Use `*` or `-` or `+`

```markdown
* Artificial Intelligence
    * Machine Learning
        * Deep Learning

- Artificial Intelligence
    - Machine Learning
        - Deep Learning

+ Artificial Intelligence
    + Machine Learning
        + Deep Learning

* Artificial Intelligence
    + Machine Learning
        - Deep Learning
```

* Artificial Intelligence
  * Machine Learning
    * Deep Learning

* Artificial Intelligence
  * Machine Learning
    * Deep Learning

* Artificial Intelligence
  * Machine Learning
    * Deep Learning

* Artificial Intelligence
  * Machine Learning
    * Deep Learning

### 5-2. Ordered Lists: Use `Number.`

```markdown
1. 1st
2. 2nd
3. 3rd
```

1. 1st
2. 2nd
3. 3rd

## 6. Blockquotes: Use `>`

```markdown
>Hello
>
>Python!
```

>Hello
>
>Python!

## 7. Tables: Use `|`

```markdown
|left-aligned|centered|right-aligned|
|:---|:---:|---:|
|Hello, Python!|Hello, Python!|Hello, Python!|
|abc|abc|abc|
```

|left-aligned|centered|right-aligned|
|:---|:---:|---:|
|Hello, Python!|Hello, Python!|Hello, Python!|
|abc|abc|abc|

## 8. Code Blocks

### 8-1. Code Blocks: Use ``` (Languages Syntax Highlighting)

* More Details: [List of languages supported by Markdown](Markdown_Code_Blocks.md)

```markdown
    ```python
    print('Hello, Python!')
    ```
```

```python
print('Hello, Python!')
```

### 8-2. Inline Code Blocks: Use `

```markdown
    Hello, `Python!`
```

Hello, `Python!`

## 9. Links

### 9-1. Links: `[Text](Links)`

```markdown
[GitHub with Links](https://github.com/)
```

[GitHub with Links](https://github.com/)

### 9-2. Inline Links

1. `[Text][Inline Links]`
2. `[Inline Links]: Links`

```markdown
[GitHub with Inline Links][Let's go GitHub]

[Let's go GitHub]: https://github.com/
```

[GitHub with Inline Links][Let's go GitHub]

[Let's go GitHub]: https://github.com/

## 10. Images

### 10-1. Images: `![Text](Image Links)`

```markdown
![GitHub Logo with Image Links](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)
```

![GitHub Logo with Image Links](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)

### 10-2. Inline Images

1. `![Tag][Text]`
2. `[Text]: Inline Image Links`

```markdown
![GitHub Logo with Inline Image Links][Let's see the GitHub logo]

[Let's see the GitHub logo]: https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png
```

![GitHub Logo with Inline Image Links][Let's see the GitHub logo]

[Let's see the GitHub logo]: https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png

## 11. Formulas

* More Details: [How to write formulas in Markdown](Markdown_LaTeX.md)

### 11-1. Left-Aligned: Use `$`

```markdown
$a^2+b^2=c^2$
```

$a^2+b^2=c^2$

### 11-2. Centered-Aligned: Use `$$`

```markdown
$$\int_\Omega \nabla u \cdot \nabla v~dx = \int_\Omega fv~dx$$
```

$$\int_\Omega \nabla u \cdot \nabla v~dx = \int_\Omega fv~dx$$

## 12. Toggle

* [How to write Markdown Toggle](https://computer-science-student.tistory.com/388)

<details>
<summary>토글 접기/펼치기</summary>
<div markdown="1">

안녕

</div>
</details>
