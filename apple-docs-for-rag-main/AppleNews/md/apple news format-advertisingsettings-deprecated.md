

- Apple News Format
-  AdvertisingSettings Deprecated

Object

# AdvertisingSettings

The object for defining properties that affect the frequency and placement with which banner advertisements and medium rectangle advertisements are automatically placed in your article.

Apple News Format 1.7–1.7Deprecated

``` source
object AdvertisingSettings
```

Deprecated

Use AdvertisementAutoPlacement instead.

## Properties

`bannerType`

`string`

The banner type that should be shown.

Default: `any`

Possible Values: `any, standard, double_height, large`

`distanceFromMedia`

`(`SupportedUnits` | integer)`

Either a number in points or a string referring to a supported unit of measure that describes the minimum required distance between automatically inserted advertisement components and media, such as video, images, and embeds.

For example, you can enter a value such as `10vh` to keep automatically inserted advertisements at 50% of the viewport height from your media content.

Version 1.1

Default: `0`

Possible types: SupportedUnits`, ``integer`

`frequency`

`integer`

A number between `0` and `10` defining the frequency for automatically inserting advertising components into articles.

Setting this value to `1` will automatically insert a banner advertisement in the first possible location below the screen bounds. Setting this value to `2` inserts a banner advertisement in the first possible location below the screen bounds, and a second banner advertisement is inserted between the first banner advertisement and the end of the article. Increasing the frequency increases the frequency of banner advertisements below the first screen bounds.

To increase the likelihood of a banner advertisement getting inserted on every screen, set the frequency to `10`. To achieve the likelihood of every other screen, set the frequency to 5.

Leaving this property out, or providing a value of `0` means that no advertisement will be inserted.

Default: `0`

Minimum: `0`

Maximum: `10`

`layout`

AdvertisingLayout

Deprecated 

Layout object that currently supports margin only. An automatically inserted advertising component uses the surrounding margins to make sure it positions itself nicely in between components. If needed, the margins that will be created around these advertisements can be defined using this layout property.

## Discussion

Use the `AdvertisingSettings` object to insert dynamic advertisements between `Body`, `Chapter`, `Section`, or `Container` components in an article.

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

### Dynamic Advertising

Managing Advertisements in Your Channel

Set the layout and frequency of ads automatically inserted in an article.

object AutoPlacement

The object for automatically placing components within Apple News Format articles.

object AdvertisementAutoPlacement

The object for defining the automatic placement of advertisements.

