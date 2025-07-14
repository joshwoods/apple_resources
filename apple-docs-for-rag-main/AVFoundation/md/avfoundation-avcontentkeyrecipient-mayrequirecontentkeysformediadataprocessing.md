

- AVFoundation
- AVContentKeyRecipient
-  mayRequireContentKeysForMediaDataProcessing 

Instance Property

# mayRequireContentKeysForMediaDataProcessing

A Boolean value that indicates whether the recipient requires decryption keys for media data to enable processing.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
var mayRequireContentKeysForMediaDataProcessing: Bool { get }
```

**Required**

## Discussion

When the value is true, adding the recipient to a content key session allows the recipient to use the session’s existing keys. It also enables handling of new key requests by the session’s delegate object.

## See Also

### Verifying Decryption Key Requirements

func contentKeySession(AVContentKeySession, didProvide: AVContentKey)

Tells the recipient that a content key is available.

