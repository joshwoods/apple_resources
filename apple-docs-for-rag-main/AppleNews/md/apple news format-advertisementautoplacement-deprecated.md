

- Apple News Format
-  AdvertisementAutoPlacement Deprecated

Object

# AdvertisementAutoPlacement

The object for defining the automatic placement of advertisements.

Apple News Format 1.9–1.25Deprecated

``` source
object AdvertisementAutoPlacement
```

## Properties

`bannerType`

`string`

A specific banner type that should be automatically inserted based on the `frequency` value. If advertisement placement is enabled, only banners of the defined size type are inserted.

Default: `any`

Possible Values: `any, standard, double_height, large`

`conditional`

`(`ConditionalAutoPlacement` | [`ConditionalAutoPlacement`])`

An instance or array of automatic placement properties that can be applied conditionally, and the conditions that cause them to take effect.

Possible types: ConditionalAutoPlacement`, ``[`ConditionalAutoPlacement`]`

`distanceFromMedia`

`(`SupportedUnits` | number)`

The minimum required distance between automatically inserted advertisement components and media, such as Video and Photo. Advertisements will show next to media if `distanceFromMedia` is not specified. To maintain a minimum distance of half a screen height from your media content, use a value of around `10vh`. For more information, see Specifying Measurements for Components.

Default: `0`

Possible types: SupportedUnits`, ``number`

`enabled`

`boolean`

A Boolean that defines whether placement of advertisements is enabled.

Default: `false`

`frequency`

`integer`

A number from `0` to `10`, defining the frequency for automatically inserting ads into articles.

Setting this value to `1` automatically inserts a dynamic advertisement in the first possible location below the screen bounds.

Setting this value to `2` inserts a dynamic advertisement in the first possible location below the screen bounds, and another between the first dynamic advertisement and the end of the article.

Increasing the frequency value increases the frequency of dynamic advertisements below the first screen bounds.

Setting this value to `0,` or omitting it, results in no advertisements.

Default: `0`

Minimum: `0`

Maximum: `10`

`layout`

AutoPlacementLayout

Deprecated 

The layout properties for automatically inserted components.

## Mentioned in 

Apple News Format Release Notes for iOS 17, iPadOS 17, and macOS 14

## Discussion

Use the `AdvertisementAutoPlacement` object to insert dynamic advertisements between Body, Chapter, Section, or Container components in an article.

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

## Relationships

### Inherits From

- AutoPlacement

## See Also

### Dynamic Advertising

Managing Advertisements in Your Channel

Set the layout and frequency of ads automatically inserted in an article.

object AutoPlacement

The object for automatically placing components within Apple News Format articles.

object AdvertisingSettings

The object for defining properties that affect the frequency and placement with which banner advertisements and medium rectangle advertisements are automatically placed in your article.

Deprecated

