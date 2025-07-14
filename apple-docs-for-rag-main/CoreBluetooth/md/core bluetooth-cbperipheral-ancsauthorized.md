

- Core Bluetooth
- CBPeripheral
-  ancsAuthorized 

Instance Property

# ancsAuthorized

A Boolean value that indicates if the remote device has authorization to receive data over ANCS protocol.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var ancsAuthorized: Bool { get }
```

## Discussion

If this value is false, a user authorization sets this value to true, which results in a call to the delegate’s centralManager(_:didUpdateANCSAuthorizationFor:) method.

