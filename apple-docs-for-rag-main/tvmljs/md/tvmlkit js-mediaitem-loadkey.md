

- TVMLKit JS
- MediaItem
-  loadKey 

Instance Property

# loadKey

A callback function used to load the security key for an item.

tvOS 9.0+

``` source
readonly attribute Object loadKey;
```

## Discussion

This attribute must be set if FairPlay Streaming is supported. The `callback` function must return either the asset identifier that was retrieved or `null`. This attribute must be assigned to a function that takes three parameters, `url`, `requestData`, and `callback`. For example, `item.loadKey = function getKey(url, requestData, callback) {}`.

The callback function must be called with the following three parameters:

1.  The key value.

2.  A renewal date, if any. If you don’t specify a renewal date, the key will not expire until the playback ends.

3.  An error parameter.

## See Also

### Supporting FairPlay Streaming

loadAssetID

A callback function used to load the asset identifier for an item.

loadCertificate

A callback function used to load the security certificate for an item.

