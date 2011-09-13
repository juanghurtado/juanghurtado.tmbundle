# Juan G. Hurtado personal TextMate bundle

## Globals

### Command: Create TOC: `^ + ⎇ + ⌘ + T`

Command that generates a Table of Content (TOC) by parsing the document for comments with this format:

```css
/* =PARENT
---------------------------------------------------------------------------------- */

... Code ...

/* =|Child
----------------------------------------- */

... Code ...

/* =|Child
----------------------------------------- */

/* =PARENT
---------------------------------------------------------------------------------- */
 
... Code ...

/* =|Child
----------------------------------------- */

... Code ...

/* =PARENT
---------------------------------------------------------------------------------- */

... Code ...

/* =|Child
----------------------------------------- */

... Code ...

/* =|Child
----------------------------------------- */

... Code ...

/* =|Child
----------------------------------------- */

... Code ...

/* =PARENT
---------------------------------------------------------------------------------- */

... Code ...
```

Resulting in a TOC like this:

```
1.PARENT
  1.1.Child
  1.2.Child
2.PARENT
  2.1.Child
3.PARENT
  3.1.Child
  3.2.Child
  3.3.Child
4.PARENT
```

### Snippet: Comment banner Header: `banh`

Creates a header comment banner:

```css
/* ----------------------------------------------------------------------------------
  Global stylesheet

  Encoding: UTF-8
  Authors:  
    Juan G. Hurtado   [hello@juanghurtado.com]
----------------------------------------------------------------------------------
  Table of contents
----------------------------------------------------------------------------------
---------------------------------------------------------------------------------- */
```

### Snippet: Comment banner: Main: `ban`

Creates a main comment banner:

```css
/* =TEXT
---------------------------------------------------------------------------------- */
```

### Snippet: Comment banner: Secondary: `bans`

Creates a secondary comment banner:

```css
/* =|Text
----------------------------------------- */
```

### Snippet: Comment banner: Method: `banm`

Creates a comment banner used for methods:

```js
/* =|foo_public_method(param)
 *  - param (type): Lorem ipsum dolor
------------------------------------------------------------------------------ */
```

## CSS

### content image: `content`

Writes the path to content images folder: `../images/content/`

### icon image: `icon`

Writes the path to icons images folder: `../images/icons/`

### layout image: `layout`

Writes the path to layout images folder: `../images/layout/`

### :focus :hover: `Shift + ⌘ + H`

Transforms selected CSS selector into a :focus :hover selector: `#content .sample a`

Into this: `#content .sample a:focus, #content .sample a:hover`

### background: none; : `bgn`

Creates a `background: none;` CSS rule.

## HTML

### ul > li * 5 > a: `ula`

Creates a sample 5 items unordered list block with links:

```html
<ul>
	<li><a href="#">Text</a></li>
	<li><a href="#">Text</a></li>
	<li><a href="#">Text</a></li>
	<li><a href="#">Text</a></li>
	<li><a href="#">Text</a></li>
</ul>
```

## Javascript

### console_log: `log`

Writes a console.log statement:

`console.log('text');`

### jQuery plugin template: `jqplugin`

Generates a sample jQuery plugin template.

### jQuery: `j`

Alias for jQuery method. Write `j`, press `Tab` and you get `jQuery`.
