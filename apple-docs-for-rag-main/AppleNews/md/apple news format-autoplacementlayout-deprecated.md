

- Apple News Format
-  AutoPlacementLayout Deprecated

Object

# AutoPlacementLayout

The object for defining the margin above and below advertising components.

Apple News Format 1.9–1.25Deprecated

``` source
object AutoPlacementLayout
```

## Properties

`margin`

`(`Margin` | integer)`

The top and bottom margin in points, or in any other unit of measure for components. See Specifying Measurements for Components.

Possible types: Margin`, ``integer`

## Mentioned in 

Apple News Format Release Notes for iOS 17, iPadOS 17, and macOS 14

## Discussion

Use the `AutoPlacementLayout` object to define the margins for ad components that are inserted automatically. This object is different from the ComponentLayout object and supports only one property, `margin`.

This object can be used in AdvertisementAutoPlacement.

### Example

```
{
  "version": "1.9",
  "identifier": "SampleArticle",
  "language": "en",
  "title": "Apple News",
  "layout": {
    "columns": 20,
    "width": 1024,
    "margin": 60,
    "gutter": 20
  },
  "autoplacement": {
    "advertisement": {
      "enabled": true,
      "bannerType": "any",
      "distanceFromMedia": "10vh",
      "frequency": 10,
      "layout": {
        "margin": 10
      }
    }
  },
  …
}
```

## See Also

### Article Layout

Planning the Layout for Your Article

Define a layout that supports the look you want for your article.

Positioning the Content in Your Article

Align article components with columns in your layout.

Wrapping Text Around a Component

Define the layout of a text component to wrap around another component.

object Layout

The object for defining columns, gutters, and margins for your article’s designed width.

object ComponentLayout

The object for defining the positioning for a specific component within the article’s column system.

object Anchor

The object for anchoring one component to another component in your article’s layout.

object Margin

The object for defining the space above and below a component.

object AdvertisingLayout

The object for defining the margin above and below advertising components.

Deprecated

