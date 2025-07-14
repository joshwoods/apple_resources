

- WebKit
- WKWebExtension
- WKWebExtension.MatchPattern
-  WKWebExtension.MatchPattern.Error 

Structure

# WKWebExtension.MatchPattern.Error

Constants that indicate errors in the WKWebExtension.MatchPattern domain.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
struct Error
```

## Topics

### Type Properties

static var errorDomain: String

static var invalidHost: WKWebExtension.MatchPattern.Error.Code

Indicates that the host component was invalid.

static var invalidPath: WKWebExtension.MatchPattern.Error.Code

Indicates that the path component was invalid.

static var invalidScheme: WKWebExtension.MatchPattern.Error.Code

Indicates that the scheme component was invalid.

static var unknown: WKWebExtension.MatchPattern.Error.Code

Indicates that an unknown error occurred.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

enum Code

Constants that indicate errors in the WKWebExtension.MatchPattern domain.

class let errorDomain: String

A string that identifies the error domain.

