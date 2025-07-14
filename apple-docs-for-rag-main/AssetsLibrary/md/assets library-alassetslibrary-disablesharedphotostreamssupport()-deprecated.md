

- Assets Library
- ALAssetsLibrary
-  disableSharedPhotoStreamsSupport() Deprecated

Type Method

# disableSharedPhotoStreamsSupport()

Disables shared photo streams notifications and asset retrieval.

iOS 6.0–9.0DeprecatediPadOS 6.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
class func disableSharedPhotoStreamsSupport()
```

Deprecated

Use the Photos framework instead

## Discussion

Shared photo streams can generate frequent notifications. Use this method to disable support if appropriate for your app.

Apps compiled against versions of iOS prior to iOS 6.0 do not have support for shared photo streams.

