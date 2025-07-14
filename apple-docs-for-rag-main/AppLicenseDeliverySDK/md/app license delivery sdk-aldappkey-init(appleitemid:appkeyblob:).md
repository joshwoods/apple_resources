

- App License Delivery SDK
- ALDAppKey
-  init(appleItemID:appKeyBlob:) 

Initializer

# init(appleItemID:appKeyBlob:)

Creates an app key to decrypt a license request.

``` source
init(
    appleItemID: UInt64,
    appKeyBlob: [UInt8]
) throws
```

## Parameters 

`appleItemID`  

A unique identifier for the app. See AppleItemID.

`appKeyBlob`  

A *key blob* for a specific app variant that App Store Connect provides your marketplace server during app ingestion. For more information, see Ingesting an alternative distribution package.

