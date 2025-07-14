

- Core Bluetooth
- CBPeripheralManagerDelegate
-  peripheralManager(\_:didAdd:error:) 

Instance Method

# peripheralManager(\_:didAdd:error:)

Tells the delegate the peripheral manager published a service to the local GATT database.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheralManager(
    _ peripheral: CBPeripheralManager,
    didAdd service: CBService,
    error: (any Error)?
)
```

## Parameters 

`peripheral`  

The peripheral manager adding the service.

`service`  

The service added to the local GATT database.

`error`  

The reason the call failed, or `nil` if no error occurred.

## Discussion

Core Bluetooth invokes this method when your app calls the add(_:) method to publish a service to the local peripheral’s GATT database. If the service published successfully to the local database, the `error` parameter is `nil`. If unsuccessful, the `error` parameter provides the cause of the failure.

