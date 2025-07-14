

- App Store Connect API
- InAppPurchaseImage
-  InAppPurchaseImage.Attributes 

Object

# InAppPurchaseImage.Attributes

Attributes that describe a subscription image resource.

App Store Connect API 3.6+

``` source
object InAppPurchaseImage.Attributes
```

## Properties

`assetToken`

`string`

`fileName`

`string`

`fileSize`

`integer`

`imageAsset`

ImageAsset

`sourceFileChecksum`

`string`

`state`

`string`

Possible Values: `AWAITING_UPLOAD, UPLOAD_COMPLETE, FAILED, PREPARE_FOR_SUBMISSION, WAITING_FOR_REVIEW, APPROVED, REJECTED`

`uploadOperations`

`[`UploadOperation`]`

## See Also

### Objects

object InAppPurchaseImage.Relationships

The data structure that represents the relationships of a subscription image resource.

