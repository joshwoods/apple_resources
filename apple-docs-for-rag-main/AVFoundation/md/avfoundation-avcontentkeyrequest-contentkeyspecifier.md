

- AVFoundation
- AVContentKeyRequest
-  contentKeySpecifier 

Instance Property

# contentKeySpecifier

The requested content key specifier.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+macOS 11.3+tvOS 14.5+visionOS 1.0+watchOS 7.4+

``` source
var contentKeySpecifier: AVContentKeySpecifier { get }
```

## See Also

### Inspecting a Request

var contentKey: AVContentKey?

The generated content key.

var options: [String : any Sendable]

A dictionary of options used to initialize key loading.

struct RetryReason

The reason for asking the client to retry a content key request.

