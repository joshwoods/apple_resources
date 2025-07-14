

- System Extensions
- OSSystemExtensionRequestDelegate
-  request(\_:actionForReplacingExtension:withExtension:) 

Instance Method

# request(\_:actionForReplacingExtension:withExtension:)

Tells the delegate that the user has a different version of the extension installed on their system.

macOS 10.15+

``` source
func request(
    _ request: OSSystemExtensionRequest,
    actionForReplacingExtension existing: OSSystemExtensionProperties,
    withExtension ext: OSSystemExtensionProperties
) -> OSSystemExtensionRequest.ReplacementAction
```

**Required**

## Parameters 

`request`  

The request that encountered a conflict.

`existing`  

A properties object that describes the installed version of the extension.

`ext`  

A properties object that describes the updated version of the extension.

## Return Value

A replacement action the manager should take to resolve the conflict.

## Mentioned in 

Installing System Extensions and Drivers

## Discussion

The manager calls this method when it encounters an existing extension with the same team and bundle identifiers, but with different version identifiers. It uses the CFBundleVersion and CFBundleShortVersionString identifiers to determine if the existing and new versions differ. The delegate must make a decision on whether to replace the existing extension.

Implement this method to return an OSSystemExtensionRequest.ReplacementAction, which tells the manager what to do. If you return OSSystemExtensionRequest.ReplacementAction.cancel, the manager aborts the installation and calls request(_:didFailWithError:), with the OSSystemExtensionError.Code.requestCanceled error code.

If the local system has System Extension developer mode enabled, the manager always calls this method when it finds an existing installation, even if the version identifiers match.

## See Also

### Handling Indeterminate Installs

func requestNeedsUserApproval(OSSystemExtensionRequest)

Tells the delegate that the user must grant approval before the manager can activate the extension.

**Required**

class OSSystemExtensionProperties

Properties that identify a specific version of a system extension.

enum ReplacementAction

Actions for describing how the extension manager should resolve a version conflict.

