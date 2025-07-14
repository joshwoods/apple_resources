

- TVMLKit JS
- MediaItem
-  loadCertificate 

Instance Property

# loadCertificate

A callback function used to load the security certificate for an item.

tvOS 9.0+

``` source
readonly attribute Object loadCertificate;
```

## Discussion

This attribute must be set if FairPlay Streaming is supported. The `callback` function must return either the asset identifier that was retrieved or `null`. This attribute must be assigned to a function that takes two parameters, `url` and `callback`; for example, `item.loadCertificate = function certificate(url, callback) {}`. The callback function must be called with the certificate that was retrieved, or with `null` as the first parameter. The second parameter is `error`. For more information, see the FairPlay Streaming page.

## See Also

### Supporting FairPlay Streaming

loadAssetID

A callback function used to load the asset identifier for an item.

loadKey

A callback function used to load the security key for an item.

