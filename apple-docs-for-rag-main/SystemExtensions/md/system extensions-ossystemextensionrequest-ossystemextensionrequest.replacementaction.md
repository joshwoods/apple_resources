

- System Extensions
- OSSystemExtensionRequest
-  OSSystemExtensionRequest.ReplacementAction 

Enumeration

# OSSystemExtensionRequest.ReplacementAction

Actions for describing how the extension manager should resolve a version conflict.

macOS 10.15+

``` source
enum ReplacementAction
```

## Topics

### Replacement Actions

case cancel

An action that tells the manager to cancel replacement of a system extension.

case replace

An action that tells the manager to replace an existing system extension.

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

### Handling Indeterminate Installs

func requestNeedsUserApproval(OSSystemExtensionRequest)

Tells the delegate that the user must grant approval before the manager can activate the extension.

**Required**

func request(OSSystemExtensionRequest, actionForReplacingExtension: OSSystemExtensionProperties, withExtension: OSSystemExtensionProperties) -> OSSystemExtensionRequest.ReplacementAction

Tells the delegate that the user has a different version of the extension installed on their system.

**Required**

class OSSystemExtensionProperties

Properties that identify a specific version of a system extension.

