

- Apple News Format
-  AutoPlacement Deprecated

Object

# AutoPlacement

The object for automatically placing components within Apple News Format articles.

Apple News Format 1.9–1.25Deprecated

``` source
object AutoPlacement
```

## Properties

`advertisement`

AdvertisementAutoPlacement

Deprecated 

The automatic placement of advertisement components. By default, no advertising is automatically inserted.

## Mentioned in 

Apple News Format Release Notes for iOS 17, iPadOS 17, and macOS 14

## Discussion

Use the `AutoPlacement` object to define the metadata, appearance, and placement of advertising components within Apple News Format articles.

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

### Inherited By

- AdvertisementAutoPlacement

## See Also

### Dynamic Advertising

Managing Advertisements in Your Channel

Set the layout and frequency of ads automatically inserted in an article.

object AdvertisementAutoPlacement

The object for defining the automatic placement of advertisements.

object AdvertisingSettings

The object for defining properties that affect the frequency and placement with which banner advertisements and medium rectangle advertisements are automatically placed in your article.

Deprecated

