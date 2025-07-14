

- AVFoundation
- AVContentKeyRequest
-  options 

Instance Property

# options

A dictionary of options used to initialize key loading.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+macOS 10.14.4+tvOS 12.2+visionOS 1.0+watchOS 7.0+

``` source
var options: [String : any Sendable] { get }
```

## See Also

### Inspecting a Request

var contentKey: AVContentKey?

The generated content key.

var contentKeySpecifier: AVContentKeySpecifier

The requested content key specifier.

struct RetryReason

The reason for asking the client to retry a content key request.

