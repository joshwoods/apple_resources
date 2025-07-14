

- Core WLAN
- CWInterface
-  startIBSSMode(withSSID:security:channel:password:) Deprecated

Instance Method

# startIBSSMode(withSSID:security:channel:password:)

Creates a computer-to-computer (ad-hoc) network with the given network name, security type, and password on the specified channel.

macOS 10.7–11.0Deprecated

``` source
func startIBSSMode(
    withSSID ssidData: Data,
    security: CWIBSSModeSecurity,
    channel: Int,
    password: String?
) throws
```

## Parameters 

`security`  

The security type to be used.

`channel`  

The channel on which the network will be created.

`password`  

The password to be used. This paramter is not applicable to open system authentication.

## Discussion

If *name* is *nil*, the machine name will be used as the network name. This operation may require an administrator password.

Handling Errors in Swift

In Swift, this method returns `Void` and is marked with the `throws` keyword to indicate that it throws an error in cases of failure.

You call this method in a `try` expression and handle any errors in the `catch` clauses of a `do` statement, as described in Error Handling in The Swift Programming Language and `About Imported Cocoa Error Parameters`.

