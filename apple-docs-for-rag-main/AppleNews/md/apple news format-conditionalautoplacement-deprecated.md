

- Apple News Format
-  ConditionalAutoPlacement Deprecated

Object

# ConditionalAutoPlacement

The object for defining conditional properties for an automatically placed component, and when the conditional properties are in effect.

Apple News Format 1.9–1.25Deprecated

``` source
object ConditionalAutoPlacement
```

## Properties

`conditions`

`(`Condition` | [`Condition`])`

 (Required) 

An instance or array of conditions that, when met, cause the conditional automatic placement properties to take effect.

Possible types: Condition`, ``[`Condition`]`

`enabled`

`boolean`

A Boolean that defines whether placement of advertisements is enabled.

Default: `false`

`layout`

AutoPlacementLayout

Deprecated 

A value that defines the layout properties for the automatically inserted components.

## Mentioned in 

Apple News Format Release Notes for iOS 17, iPadOS 17, and macOS 14

## Discussion

Use the `ConditionalAutoPlacement` object to define an array of conditional automatic placement properties and the conditions under which to apply them. When a condition is met, the value of a property in `ConditionalAutoPlacement` overrides the value of the same property if defined in the parent `AdvertisementAutoPlacement` object. See AdvertisementAutoPlacement.

### Example

```
{
  "version": "1.9",
  "identifier": "SampleArticle",
  "language": "en",
  "title": "Apple News",
  "layout": {
    "columns": 7,
    "width": 1024,
    "margin": 75,
    "gutter": 20
  },
  "autoplacement": {
    "advertisement": {
      "enabled": true,
      "bannerType": "any",
      "distanceFromMedia": "50vh",
      "frequency": 10,
      "layout": {
        "margin": 10
      },
      "conditional": [
        {
          "enabled": false,
          "conditions": [
            {
              "verticalSizeClass": "compact"
            }
          ]
        }
      ]
    }
  },
  …
}
```

## See Also

### Conditional Design Elements

object Condition

The object for defining a condition that, when met, causes conditional properties to go into effect.

object ConditionalComponent

The object for defining conditional properties for a component, and when the conditional properties are in effect.

object ConditionalComponentLayout

The object for defining conditional properties for a component layout, and when the conditional properties are in effect.

object ConditionalSection

The object for defining conditional properties for a section component, and when the conditional properties are in effect.

object ConditionalDocumentStyle

The object for defining conditional properties for a document style, and when the conditional properties are in effect.

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

