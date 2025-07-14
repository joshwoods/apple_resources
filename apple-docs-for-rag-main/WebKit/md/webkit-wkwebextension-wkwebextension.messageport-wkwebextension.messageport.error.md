

- WebKit
- WKWebExtension
- WKWebExtension.MessagePort
-  WKWebExtension.MessagePort.Error 

Structure

# WKWebExtension.MessagePort.Error

Constants that indicate errors in the WKWebExtension.MessagePort domain.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
struct Error
```

## Topics

### Type Properties

static var errorDomain: String

A string that identifies the error domain.

static var messageInvalid: WKWebExtension.MessagePort.Error.Code

Indicates that the message is invalid.

static var notConnected: WKWebExtension.MessagePort.Error.Code

Indicates that the message port is disconnected.

static var unknown: WKWebExtension.MessagePort.Error.Code

Indicates that an unknown error occurred.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

