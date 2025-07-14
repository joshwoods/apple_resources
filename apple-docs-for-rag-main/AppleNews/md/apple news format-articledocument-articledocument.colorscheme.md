

- Apple News Format
- ArticleDocument
-  ArticleDocument.colorScheme 

Object

# ArticleDocument.colorScheme

The object that contains information about the color scheme of the document, including Dark Mode behavior.

Apple News Format 1.14.1+

``` source
object ArticleDocument.colorScheme
```

## Properties

`automaticDarkModeEnabled`

`boolean`

A Boolean value that indicates whether automatic Dark Mode is enabled for the document. The value for this property defaults to `true`, which causes the document to be inverted when the user switches the device to Dark Mode.

Default: `true`

## Discussion

Use the c`olorScheme` object to enable or disable automatic Dark Mode in a document.

### Example

```
{
 "version": "1.14.1",
 "identifier": "SampleArticle",
 "language": "en",
 "title": "Apple News",
 "subtitle": "A look at the features of Apple News",
 "layout": {
   "columns": 20,
   "width": 1024,
   "margin": 60,
   "gutter": 20
 },
 …
 "colorScheme": {
   "automaticDarkModeEnabled": true
 }
}
```

## See Also

### Objects

object ArticleDocument.componentLayouts

An object containing component layout objects that components in the article can refer to.

object ArticleDocument.componentStyles

An object containing component style objects that components in the article can refer to.

object ArticleDocument.componentTextStyles

An object containing component text style defaults as well as component text styles that components in the article can use.

object ArticleDocument.textStyles

An object containing text style objects that components within this document can refer to inline in text.

