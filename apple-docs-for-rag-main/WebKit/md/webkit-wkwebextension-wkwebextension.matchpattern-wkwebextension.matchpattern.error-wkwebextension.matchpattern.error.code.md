

- WebKit
- WKWebExtension
- WKWebExtension.MatchPattern
- WKWebExtension.MatchPattern.Error
-  WKWebExtension.MatchPattern.Error.Code 

Enumeration

# WKWebExtension.MatchPattern.Error.Code

Constants that indicate errors in the WKWebExtension.MatchPattern domain.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
enum Code
```

## Topics

### Enumeration Cases

case invalidHost

Indicates that the host component was invalid.

case invalidPath

Indicates that the path component was invalid.

case invalidScheme

Indicates that the scheme component was invalid.

case unknown

Indicates that an unknown error occurred.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

struct Error

Constants that indicate errors in the WKWebExtension.MatchPattern domain.

class let errorDomain: String

A string that identifies the error domain.

