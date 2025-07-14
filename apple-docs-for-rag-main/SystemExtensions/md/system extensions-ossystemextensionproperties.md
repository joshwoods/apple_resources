

- System Extensions
-  OSSystemExtensionProperties 

Class

# OSSystemExtensionProperties

Properties that identify a specific version of a system extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 10.15+

``` source
class OSSystemExtensionProperties
```

## Topics

### Identifying the Extension

var bundleIdentifier: String

The bundle identifier of the extension.

var bundleVersion: String

The bundle version of the extension.

var bundleShortVersion: String

The bundle short version string of the extension.

### Locating the Extension’s Installed Location

var url: URL

The file URL of the extension bundle.

### Instance Properties

var isAwaitingUserApproval: Bool

var isEnabled: Bool

var isUninstalling: Bool

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Handling Indeterminate Installs

func requestNeedsUserApproval(OSSystemExtensionRequest)

Tells the delegate that the user must grant approval before the manager can activate the extension.

**Required**

func request(OSSystemExtensionRequest, actionForReplacingExtension: OSSystemExtensionProperties, withExtension: OSSystemExtensionProperties) -> OSSystemExtensionRequest.ReplacementAction

Tells the delegate that the user has a different version of the extension installed on their system.

**Required**

enum ReplacementAction

Actions for describing how the extension manager should resolve a version conflict.

