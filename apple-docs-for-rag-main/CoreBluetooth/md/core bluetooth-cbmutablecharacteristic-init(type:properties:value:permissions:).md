

- Core Bluetooth
- CBMutableCharacteristic
-  init(type:properties:value:permissions:) 

Initializer

# init(type:properties:value:permissions:)

Creates a mutable characteristic with specified permissions, properties, and value.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+

``` source
init(
    type UUID: CBUUID,
    properties: CBCharacteristicProperties,
    value: Data?,
    permissions: CBAttributePermissions
)
```

## Parameters 

`UUID`  

A 128-bit UUID that identifies the characteristic.

`properties`  

The properties of the characteristic.

`value`  

The characteristic value to cache. If `nil`, the value is dynamic and the peripheral manager fetches it on demand.

`permissions`  

The permissions of the characteristic value.

## Return Value

A newly initialized mutable characteristic.

## Discussion

If you specify a value for the characteristic, the characteristic caches the value and sets its properties and permissions to read and readable, respectively. Therefore, if you need the value of a characteristic to be writeable, or if you expect the value to change during the lifetime of the published service to which the characteristic belongs, you must specify the value as `nil`. This ensures that the characteristic treats the value dynamically. With a dynamic value, the peripheral manager requests the value whenever the peripheral manager receives a read or write request from a central. The peripheral does this by calling the peripheralManager(_:didReceiveRead:) and peripheralManager(_:didReceiveWrite:) methods of its delegate object, respectively.

For more information, see Core Bluetooth Programming Guide.

