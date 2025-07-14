

- Apple News Format
- ArticleDocument
-  ArticleDocument.componentStyles 

Object

# ArticleDocument.componentStyles

An object containing component style objects that components in the article can refer to.

Apple News Format 1.7+

``` source
object ArticleDocument.componentStyles
```

## Properties

`Any Key`

ComponentStyle

A component style, with a name you define that components within this document can refer to.

## Mentioned in 

Enhancing Your Articles with Styles

Defining a Component Style

## Discussion

`ArticleDocument.componentStyles` is an object containing the component style objects that components in your article can use. You provide each component style object as a key-value pair. In each pair, you create a key that’s meaningful to you. The value of each pair is a ComponentStyle object.

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
    "backgroundColor": "#FFFFFF"
  },
  "components": [
    {
      "role": "section",
      "style": "exampleStyle",
      "components": [
        {
          "role": "body",
          "text": "Apple News Format allows publishers to craft beautiful editorial layouts. Galleries, audio, video, and fun interactions like animation make stories spring to life.",
          "layout": {
            "margin": {
              "top": 10,
              "bottom": 10
            }
          }
        }
      ]
    }
  ],
  "componentTextStyles": {},
  "textStyles": {},
  "componentStyles": {
    "exampleStyle": {
      "backgroundColor": "#FFFFFF",
      "opacity": 1,
      "border": {
        "all": {
          "width": 1,
          "color": "black"
        },
        "left": false,
        "right": false
      }
    }
  },
  "componentLayouts": {}
}
```

## See Also

### Objects

object ArticleDocument.componentLayouts

An object containing component layout objects that components in the article can refer to.

object ArticleDocument.componentTextStyles

An object containing component text style defaults as well as component text styles that components in the article can use.

object ArticleDocument.textStyles

An object containing text style objects that components within this document can refer to inline in text.

object ArticleDocument.colorScheme

The object that contains information about the color scheme of the document, including Dark Mode behavior.

