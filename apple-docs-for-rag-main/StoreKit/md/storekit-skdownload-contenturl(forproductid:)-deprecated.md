

- StoreKit
- SKDownload
-  contentURL(forProductID:) Deprecated

Type Method

# contentURL(forProductID:)

Returns the local location for the previously downloaded flie.

Mac Catalyst 13.0–16.0DeprecatedmacOS 10.8–13.0Deprecated

``` source
class func contentURL(forProductID productID: String) -> URL?
```

Deprecated

Hosted content is no longer supported

## Parameters 

`productID`  

The product identifier.

## Return Value

The local location for the previously downloaded flie.

## Mentioned in 

Unlocking purchased content

## Discussion

Use this method to locate the content on subsequent launches of your app.

## See Also

### Managing Downloaded Content

class func deleteContent(forProductID: String)

Deletes the previously downloaded file.

Deprecated

