

- System Extensions
- OSSystemExtensionRequestDelegate
-  requestNeedsUserApproval(\_:) 

Instance Method

# requestNeedsUserApproval(\_:)

Tells the delegate that the user must grant approval before the manager can activate the extension.

macOS 10.15+

``` source
func requestNeedsUserApproval(_ request: OSSystemExtensionRequest)
```

**Required**

## Discussion

Activating an extension may require explicit user approval to proceed. For example, this occurs when the user hasn’t approved the extension. The manager calls this method to notify the delegate. Activation remains pending until the user grants or denies permission, or until the app quits.

## See Also

### Handling Indeterminate Installs

func request(OSSystemExtensionRequest, actionForReplacingExtension: OSSystemExtensionProperties, withExtension: OSSystemExtensionProperties) -> OSSystemExtensionRequest.ReplacementAction

Tells the delegate that the user has a different version of the extension installed on their system.

**Required**

class OSSystemExtensionProperties

Properties that identify a specific version of a system extension.

enum ReplacementAction

Actions for describing how the extension manager should resolve a version conflict.

