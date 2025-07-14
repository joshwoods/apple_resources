

- WebKit
- WKWebExtension
- WKWebExtension.DataRecord
-  WKWebExtension.DataRecord.Error 

Structure

# WKWebExtension.DataRecord.Error

Constants that indicate errors in the WKWebExtension.DataRecord domain.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
struct Error
```

## Topics

### Type Properties

static var errorDomain: String

Indicates a WKWebExtension.DataRecord error.

static var localStorageFailed: WKWebExtension.DataRecord.Error.Code

Indicates a failure occurred when either deleting or calculating local storage.

static var sessionStorageFailed: WKWebExtension.DataRecord.Error.Code

Indicates a failure occurred when either deleting or calculating session storage.

static var synchronizedStorageFailed: WKWebExtension.DataRecord.Error.Code

Indicates a failure occurred when either deleting or calculating synchronized storage.

static var unknown: WKWebExtension.DataRecord.Error.Code

Indicates that an unknown error occurred.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

