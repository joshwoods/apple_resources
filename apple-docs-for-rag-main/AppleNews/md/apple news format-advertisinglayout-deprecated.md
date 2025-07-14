

- Apple News Format
-  AdvertisingLayout Deprecated

Object

# AdvertisingLayout

The object for defining the margin above and below advertising components.

Apple News Format 1.7–1.7Deprecated

``` source
object AdvertisingLayout
```

Deprecated

Use AutoPlacementLayout instead.

## Properties

`margin`

`(`Margin` | integer)`

 (Required) 

Describes margins on top and bottom as a single integer or as an object containing separate properties for top and bottom margins.

Version 1.1

Possible types: Margin`, ``integer`

## Discussion

Define the margins for the BannerAdvertisement components that are inserted automatically. This object is different from the ComponentLayout object and supports only one property, `margin`.

This object can be used in AdvertisingSettings.

### Example

```
{
  "advertisingSettings": {
    "frequency": 10,
    "layout": {
      "margin": {
        "top": 15,
        "bottom": 20
      }
    }
  }
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

object AutoPlacementLayout

The object for defining the margin above and below advertising components.

