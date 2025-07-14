

- CallKit
- CXCallDirectoryManager
-  CXCallDirectoryManager.EnabledStatus 

Enumeration

# CXCallDirectoryManager.EnabledStatus

The enabled status of a Call Directory app extension, as reported by the getEnabledStatusForExtension(withIdentifier:completionHandler:) method.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+

``` source
enum EnabledStatus
```

## Topics

### Constants

case unknown

Indicates that the enabled status for the extension is unknown.

case disabled

Indicates that the extension is disabled.

case enabled

Indicates that the extension is enabled.

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

### Working with a Call Directory App Extension

func getEnabledStatusForExtension(withIdentifier: String, completionHandler: (CXCallDirectoryManager.EnabledStatus, (any Error)?) -> Void)

Asynchronously returns the enabled status of the extension with the specified identifier.

func reloadExtension(withIdentifier: String, completionHandler: (((any Error)?) -> Void)?)

Asynchronously reloads the extension with the specified identifier.

