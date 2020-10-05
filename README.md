## New Economic School Logo

`neslogo` is a package which implements the `\neslogo` LaTeX macro.
It puts a [New Economic School](https://www.nes.ru) logo into a document.

There is an example document which shows several variants of the logo.

## Installation

Just put `neslogo.sty` and `neslogofallback.sty` into your TEXMF tree,
typically eithe into `%USERPROFILE%/texmf/tex/latex/neslogo/` (on MS Windows),
or into `$HOME/texmf/tex/latex/neslogo/` on Linux.

## Usage

Put into your document's preamble

```
\usepackage{neslogo}
```

and then `\neslogo` will place a one-inch height logo into the document.
The macro supports several optional parameters:

<dl>
<dt>`lang`</dt>
<dd>(`russian` or `english`) Choose the logo language</dd>
<dt>`size`</dt>
<dd>(any LaTeX length, like `2cm`) Choose the height of the logo</dd>
<dt>`palette`</dt>
<dd>(`color`, `grey`, or `mono`) Choose the logo palette</dd>
<dt>`color`</dt>
<dd>(`black`, `white`, `blue`, `red`, `lightgrey`, or `darkgrey`) If the `palette` is `color` or `grey`, choose
the color of the logo text (only `black` and `white` make sense here, `black` for white background, and
`white` for black background), If the `palette` is `mono`, then it makes the color of the logo
(the NES brandbook prescribes only `white`, `black` and `blue` logos, but any other three colors are
supported as well).</dd>
</dl>

## Examples

`\neslogo[lang=english,palette=color,color=white]`
`\neslogo[lang=russian,palette=mono,color=blue]`

