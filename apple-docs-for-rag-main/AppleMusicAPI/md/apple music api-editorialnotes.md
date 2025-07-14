

- Apple Music API
-  EditorialNotes 

Object

# EditorialNotes

An object that represents a notes attribute.

Apple Music 1.0+

``` source
object EditorialNotes
```

## Properties

`short`

`string`

Abbreviated notes shown inline or when the content appears alongside other content.

`standard`

`string`

Notes shown when the content is prominently displayed.

`name`

`string`

Name for the editorial notes.

`tagline`

`string`

The tag line for the editorial notes.

## Discussion

Notes may include XML tags for formatting (`` for bold, `` for italic, or `` for line break) and special characters (`&amp;` for `&`, `&lt;` for ``, `&apos;` for `‘`, and `&quot;` for `“`).

