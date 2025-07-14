

- AVFoundation
- AVContentKeyRecipient
-  contentKeySession(\_:didProvide:) 

Instance Method

# contentKeySession(\_:didProvide:)

Tells the recipient that a content key is available.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.4+

``` source
optional func contentKeySession(
    _ contentKeySession: AVContentKeySession,
    didProvide contentKey: AVContentKey
)
```

## Parameters 

`contentKeySession`  

The current content key session.

`contentKey`  

A content key to use with objects that support manual attachment of keys, such as doc://com.apple.documentation/documentation/coremedia/cmsamplebuffer-u71.

## See Also

### Verifying Decryption Key Requirements

var mayRequireContentKeysForMediaDataProcessing: Bool

A Boolean value that indicates whether the recipient requires decryption keys for media data to enable processing.

**Required**

