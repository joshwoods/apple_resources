

- Service Management
-  SMLoginItemSetEnabled(\_:\_:) Deprecated

Function

# SMLoginItemSetEnabled(\_:\_:)

Enables a helper executable in the main app-bundle directory.

macOS 10.6–13.0Deprecated

``` source
func SMLoginItemSetEnabled(
    _ identifier: CFString,
    _ enabled: Bool
) -> Bool
```

Deprecated

Please use SMAppService instead

## Parameters 

`identifier`  

The identifier of the helper executable bundle.

`enabled`  

A Boolean value that represents the state of the helper executable. This value is effective only for the currently logged-in user. If true, the helper tool executable immediately (and upon subsequent logins) and keeps running. If false, the helper executable stops.

## Return Value

Returns true if the requested change has taken effect.

## Discussion

Important

To enable or disable `LoginItems` in macOS 13 and later, use the register() and unregister() methods instead.

The build system places helper executables in the app’s bundle in the `Contents/Library/LoginItems` directory.

