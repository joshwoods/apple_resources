

- Apple News Format
-  ConditionalDocumentStyle 

Object

# ConditionalDocumentStyle

The object for defining conditional properties for a document style, and when the conditional properties are in effect.

Apple News Format 1.10.1+

``` source
object ConditionalDocumentStyle
```

## Properties

`conditions`

`(`Condition` | [`Condition`])`

 (Required) 

An instance or array of conditions that, when met, cause the conditional document style properties to take effect.

Possible types: Condition`, ``[`Condition`]`

`backgroundColor`

Color

The document’s background color. The value defaults to white.

## Mentioned in 

Supporting Dark Mode for Your Article

## Discussion

Use the `ConditionalDocumentStyle` object to define an array of conditional document-style properties and the conditions under which to apply them. When a condition is met, the value of a property in `ConditionalDocumentStyle` overrides the value of the same property if defined in the parent `DocumentStyle` object. See DocumentStyle.

### Example

```
{
  "documentStyle": {
    "backgroundColor": "#FFF",
    "conditional": [
      {
        "backgroundColor": "#000",
        "conditions": [
          {
            "preferredColorScheme": "dark"
          }
        ]
      }
    ]
  },
  "components": [
    {
      "role": "title",
      "text": "Apple News Format"
    },
    {
      "role": "body",
      "text": "Apple News Format allows publishers to craft beautiful editorial layouts. Galleries, audio, video, and fun interactions like animation make stories spring to life."
    },
    {
      "role": "photo",
      "URL": "bundle://image.jpg"
    }
  ]
}
```

## Relationships

### Inherits From

- DocumentStyle

## See Also

### Conditional Design Elements

object Condition

The object for defining a condition that, when met, causes conditional properties to go into effect.

object ConditionalComponent

The object for defining conditional properties for a component, and when the conditional properties are in effect.

object ConditionalComponentLayout

The object for defining conditional properties for a component layout, and when the conditional properties are in effect.

object ConditionalAutoPlacement

The object for defining conditional properties for an automatically placed component, and when the conditional properties are in effect.

object ConditionalSection

The object for defining conditional properties for a section component, and when the conditional properties are in effect.

object ConditionalText

The object for defining conditional properties for a text component, and when the conditional properties are in effect.

object ConditionalTextStyle

The object for defining conditional properties for a text style, and when the conditional properties are in effect.

object ConditionalComponentTextStyle

The object for defining conditional properties for a component text style, and when the conditional properties are in effect.

object ConditionalComponentStyle

The object for defining conditional properties for a component style, and when the conditional properties are in effect.

object ConditionalContainer

The object for defining conditional properties for a container component, and when the conditional properties are in effect.

object ConditionalDivider

The object for defining conditional properties for a divider component, and when the conditional properties are in effect.

object ConditionalButton

The object for defining a button component’s conditional properties, and when the conditional properties are in effect.

