

- Core Bluetooth
- CBCentralManagerDelegate
-  centralManager(\_:didUpdateANCSAuthorizationFor:) 

Instance Method

# centralManager(\_:didUpdateANCSAuthorizationFor:)

Tells the delegate the authorization status changed for a ANCS-requiring connected peripheral.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
optional func centralManager(
    _ central: CBCentralManager,
    didUpdateANCSAuthorizationFor peripheral: CBPeripheral
)
```

## Parameters 

`central`  

The central manager providing this information.

`peripheral`  

The CBPeripheral that caused the event.

