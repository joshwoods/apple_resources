

- WebKit
- WKWebExtensionContext
-  WKWebExtensionContext.Error 

Structure

# WKWebExtensionContext.Error

Constants used to indicate errors in the web extension context domain.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
struct Error
```

## Topics

### Type Properties

static var alreadyLoaded: WKWebExtensionContext.Error.Code

Indicates that the context is already loaded by a WKWebExtensionController.

static var backgroundContentFailedToLoad: WKWebExtensionContext.Error.Code

Indicates that an error occurred loading the background content.

static var baseURLAlreadyInUse: WKWebExtensionContext.Error.Code

Indicates that another context is already using the specified base URL.

static var errorDomain: String

A string that identifies the error domain.

static var noBackgroundContent: WKWebExtensionContext.Error.Code

Indicates that the extension does not have background content.

static var notLoaded: WKWebExtensionContext.Error.Code

Indicates that the context is not loaded by a WKWebExtensionController.

static var unknown: WKWebExtensionContext.Error.Code

Indicates that an unknown error occurred.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Structures

struct NotificationUserInfoKey

Constants for specifying web extension context information in notifications.

