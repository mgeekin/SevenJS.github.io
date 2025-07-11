# [SevenJS : 7 function frontend library](SevenJS.github.io)

SevenJS formerly known as [GeneratorJS](https://generatorjs.github.io)

Frontend design with less typing, less editing to HTML CSS  
With only **Seven** functions.

## Install SevenJS

```bash
# https://github.com/mgeekin/SevenJS.init.git
git clone https://github.com/mgeekin/SevenJS.init.git
```
# Add script in html directly

### Current version v0.9.1
```html
<script src="https://sevenjs.github.io/release/v0.9.1/seven.min.js" defer></script>
```
or 

### Latest version
```html
<script src="https://sevenjs.github.io/release/latest/seven.min.js" defer></script>
```


---

# Learn seven functions of SevenJS

1. [gen](#gen)
2. [append](#append)
3. [grab](#grab)   
4. [load](#laod)
5. [loadscss](#loadscss)
6. [parsemd](#parsemd)
7. [cssvar](#cssvar)
* [getfile](#getfile)
* [log](#log)

---
## #gen

To create HTML element from JS by specifying tag, id, content, classes, and attributes.
```js
gen((tag, id, content, classes, attributes)
```

- tag: all html tags like p,h1,span, div etc.
- id: desired id of html tag (skipped with empty string ``).
- content: text, html, or another html element, or an array of text, html, or another html element (skipped with empty string ``).
- classes: list of classes in a string seprated by coma or space (skipped with empty string ``).
- attributes: optional, for some tags it is some nessary component url, link etc, in generic cases all it can be a dictionary of key-value pairs, each key for attribute name and value for attribute value say {"onclick":"clickfunction()", "data-roll":10} 

|Desired element in DOM| Required code|
|:---|---:|
|`<p>hi</p>`|`gen("p", "", "hi")`|
|`<p id="greet">hi</p>`|`gen("p", "greet", "hi")`|
|`<p id="greet" class="bold red">hi</p>`|`gen("p", "greet", "hi","bold,red")`|
|`<p id="greet" class="bold red" onclick="clickfunction()">hi</p>`|`gen("p", "greet", "hi","bold,red",{"onclick":"clickfunction()"})`|
|`<p><span>hello</span></p>`|`gen("p", "", gen("span","","hello"))`|
|`<a id="link" class="linkclass" href="url">linkname</a>`|`gens(a,"link","linkname","linkclass","url")`|
|`<li>link1</li><li>link2</li><li>link3</li>`|`gen(li,"",["link1","link2","link3"])`|

---
## #append

---
## #grab

---
## #load

---
## #loadscss

---
## #parsemd

---
## #cssvar

---
### #getfile

---
### #log

--- 

# Learn by Examples

[SevenJS.github.io/examples](https://SevenJS.github.io/examples)
