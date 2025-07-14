

- Core Bluetooth
- CBPeripheralManagerDelegate
-  peripheralManagerDidStartAdvertising(\_:error:) 

Instance Method

# peripheralManagerDidStartAdvertising(\_:error:)

Tells the delegate the peripheral manager started advertising the local peripheral device’s data.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheralManagerDidStartAdvertising(
    _ peripheral: CBPeripheralManager,
    error: (any Error)?
)
```

## Parameters 

`peripheral`  

The peripheral manager that is starting advertising.

`error`  

The reason the call failed, or `nil` if no error occurred.

## Discussion

Core Bluetooth calls this method when your app calls the startAdvertising(_:) method to advertise the local peripheral device’s data. If successful, the `error` parameter is `nil`. If a problem prevents advertising the data, the `error` parameter returns the cause of the failure.

