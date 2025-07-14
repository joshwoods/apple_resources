

- Device Management
- Apps
- Apps.Attributes
-  Apps.Attributes.Offers 

Object

# Apps.Attributes.Offers

Device Assignment ServicesVPP License Management

``` source
object Apps.Attributes.Offers
```

## Properties

`assets`

`[`Apps.Attributes.Offers.Assets`]`

`buyParams`

`string`

`currencyCode`

`string`

`discounts`

`[`Apps.Attributes.Offers.Discounts`]`

`download`

Apps.Attributes.Offers.Download

`expectedReleaseDate`

`string`

`offerSummary`

`string`

`price`

`number`

`priceFormatted`

`string`

`pricePerUnit`

`number`

`pricePerUnitFormatted`

`string`

`quantity`

`integer`

`recurringSubscriptionPeriod`

`string`

`type`

`string`

 (Required) 

Possible Values: `anonymousDownload, buy, complete, get, preorder, preordered, purchased, radio, redownload, rent, subscribe, subscription, update`

## Topics

### Related Objects

object Apps.Attributes.Offers.Assets

object Apps.Attributes.Offers.Discounts

object Apps.Attributes.Offers.Download

## See Also

### Related Objects

object Apps.Attributes.ContentRatingsBySystem

object Apps.Attributes.FileSizeByDevice

object Apps.Attributes.LatestVersionInfo

object Apps.Attributes.RequirementsByDeviceFamily

object Apps.Attributes.ScreenshotsByType

object Apps.Attributes.TaxExclusivePrices

object Apps.Attributes.UserRating

object Apps.Attributes.VersionHistory

