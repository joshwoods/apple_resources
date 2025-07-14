

- WebKit
- WKWebExtensionContext
-  WKWebExtensionContext.PermissionStatus 

Enumeration

# WKWebExtensionContext.PermissionStatus

Constants used to indicate permission status in web extension context.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
enum PermissionStatus
```

## Topics

### Enumeration Cases

case deniedExplicitly

Indicates that the permission was explicitly denied.

case deniedImplicitly

Indicates that the permission was implicitly denied because of another explicitly denied permission.

case grantedExplicitly

Indicates that the permission was explicitly granted permission.

case grantedImplicitly

Indicates that the permission was implicitly granted because of another explicitly granted permission.

case requestedExplicitly

Indicates that the permission was explicitly requested.

case requestedImplicitly

Indicates that the permission was implicitly requested because of another explicitly requested permission.

case unknown

Indicates an unknown permission status.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

