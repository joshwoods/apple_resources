

- Apple News Format
- ArticleDocument
-  ArticleDocument.textStyles 

Object

# ArticleDocument.textStyles

An object containing text style objects that components within this document can refer to inline in text.

Apple News Format 1.7+

``` source
object ArticleDocument.textStyles
```

## Properties

`Any Key`

TextStyle

A text style, with a name you define that components within this document can refer to.

## Mentioned in 

Enhancing Your Articles with Styles

Defining and Applying Text Styles

Using HTML with Apple News Format

## Discussion

`Article Document.textStyles` is an object containing the text style objects that components in your article can refer to inline from their text, using HTML or Markdown. See Using HTML with Apple News Format and Using Markdown with Apple News Format. You can also refer to these text style objects in an InlineTextStyle object within a component.

You provide each component layout object as a key-value pair. In each pair, you create a key that’s meaningful to you. The value of each pair is a TextStyle object.

### Example

```
{
  "title": "Article Title",
  "identifier": "sample",
  "version": "1.8",
  "language": "en",
  "layout": {
    "columns": 20,
    "width": 1024,
    "margin": 60,
    "gutter": 20
  },
  "documentStyle": {
    "backgroundColor": "#FFF"
  },
  "components": [
    {
      "role": "section",
      "components": [
        {
          "role": "body",
          "format": "html",
          "text": "There is a moment in every dawn when light floats, there is the possibility of magic. Creation holds its breath."
        }
      ]
    }
  ],
  "componentTextStyles": {},
  "textStyles": {
    "exampleStyle": {
      "fontFamily": "Gill Sans",
      "fontWeight": "bolder",
      "textColor": "#333333",
      "fontSize": 18,
      "textShadow": {
        "radius": 20,
        "opacity": 0.3,
        "color": "#99999930",
        "offset": {
          "x": -10,
          "y": 5
        }
      },
      "stroke": {
        "color": "#FFC800",
        "width": 1
      }
    }
  },
  "componentStyles": {},
  "componentLayouts": {}
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

object ArticleDocument.colorScheme

The object that contains information about the color scheme of the document, including Dark Mode behavior.

