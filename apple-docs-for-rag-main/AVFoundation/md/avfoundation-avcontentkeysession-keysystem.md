

- AVFoundation
- AVContentKeySession
-  keySystem 

Instance Property

# keySystem

The type of key system used to retrieve keys.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
var keySystem: AVContentKeySystem { get }
```

## Discussion

Valid values for keySystem are fairPlayStreaming and clearKey.

## See Also

### Inspecting the Session

struct AVContentKeySystem

A key-delivery method for a content key session.

var storageURL: URL?

A URL that points to a writable storage directory.

