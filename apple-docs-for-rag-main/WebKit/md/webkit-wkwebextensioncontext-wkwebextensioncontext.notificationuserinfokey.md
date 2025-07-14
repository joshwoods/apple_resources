

- WebKit
- WKWebExtensionContext
-  WKWebExtensionContext.NotificationUserInfoKey 

Structure

# WKWebExtensionContext.NotificationUserInfoKey

Constants for specifying web extension context information in notifications.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
struct NotificationUserInfoKey
```

## Topics

### Type properties

static let matchPatterns: WKWebExtensionContext.NotificationUserInfoKey

The corresponding value represents the affected permission match patterns in WKWebExtensionContext notifications.

static let permissions: WKWebExtensionContext.NotificationUserInfoKey

The corresponding value represents the affected permissions in WKWebExtensionContext notifications.

### Initializers

init(String)

Creates a constant from a value you provide.

init(rawValue: String)

Creates a constant from a raw value you provide.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Structures

struct Error

Constants used to indicate errors in the web extension context domain.

