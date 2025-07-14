

- TVMLKit JS
- MediaItem
-  loadAssetID 

Instance Property

# loadAssetID

A callback function used to load the asset identifier for an item.

tvOS 9.0+

``` source
readonly attribute Object loadAssetID;
```

## Discussion

This attribute must be set if FairPlay Streaming is supported. This attribute must be assigned to a function that takes two parameters, `url` and `callback`; for example, `item.loadAssetID = function assetID(url, callback) {}`. The callback function must be called with the asset identifier that was retrieved, or with `null` as the first parameter. The second parameter is `error`. For more information, see the FairPlay Streaming page.

## See Also

### Supporting FairPlay Streaming

loadCertificate

A callback function used to load the security certificate for an item.

loadKey

A callback function used to load the security key for an item.

