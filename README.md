[//]: # (Copyright 2018 Alice Charlotte Liddell)

[//]: # (Licensed under the Apache License, Version 2.0, henceforth the "License";)

[//]: # (you may not use this file except in compliance with the License.)
[//]: # (You may obtain a copy of the License at)

[//]: # (http://www.apache.org/licenses/LICENSE-2.0)

[//]: # (Unless required by applicable law or agreed to in writing, software)
[//]: # (distributed under the License is distributed on an "AS IS" BASIS,)
[//]: # (WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.)
[//]: # (See the License for the specific language governing permissions and)
[//]: # (limitations under the License.)

# Markdown tricks

GitHub allows us to use a limited subset of HTML in our Markdown files – let's see what mischief we can do with that and even more!
This collection of hacks contains the solutions of the (un)common problems I've encountered.

> **Note:** These tricks don't show up when you "Preview changes", you have to actually commit and view in the GitHub web UI or use a local renderer to see it.

## Alignment

<div align="center">This is center aligned!</div>
<div align="left">Left aligned</div>
<div align="right">Right aligned</div>

```HTML
<div align="center">This is center aligned!</div>
<div align="left">Left aligned</div>
<div align="right">Right aligned</div>
```

## Commenting

> **Note:** These comments are NOT visible in previews/rendered documents and are similar to those of the other programming languages

[//]: # (This is a comment)
[//]: # (And another one)
[//]: # (You can't see this text, unless you look at the document source)

```Markdown
[//]: # (This is a comment)
[//]: # (And another one)
[//]: # (You can't see this text, unless you look at the document source)
```

## Dropdowns

<details>

<summary>Click Me</summary>

- Example entry one
- Example entry two
- Example entry three
- Example entry four
- Example entry five

</details>

```Markdown
<details>

<summary>Click Me</summary>

- Example entry one
- Example entry two
- Example entry three
- Example entry four
- Example entry five

</details>
```

## Hanging indendation

<dl>
  <dt>This is a list</dt>
  <dd>With hanging indentation</dd>

  <dt>Another list item</dt>
  <dd>With some description that might wrap over more than one line hopefully. This is to showcase that the hanging indentation persists even with a very long description and a bunch of line breaks!</dd>
</dl>

```HTML
<dl>
  <dt>This is a list</dt>
  <dd>With hanging indentation</dd>
</dl>
```

## Line breaks

If you need a line break, just put two spaces at its end.

This is a simple poem  
Intended to process  
The code that can be stolen  
In order to impress

## Mouseover text

<span style="text-decoration:underline" title="This is how you can do it">Mouseover</span>

```HTML
<span style="text-decoration:underline" title="This is how you can do it">Mouseover</span>
```

## Tables

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

```Markdown
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

