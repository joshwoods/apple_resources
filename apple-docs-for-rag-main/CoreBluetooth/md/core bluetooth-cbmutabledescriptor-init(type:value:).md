

- Core Bluetooth
- CBMutableDescriptor
-  init(type:value:) 

Initializer

# init(type:value:)

Creates a mutable descriptor with a specified value.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+

``` source
init(
    type UUID: CBUUID,
    value: Any?
)
```

## Parameters 

`UUID`  

A 128-bit UUID that identifies the characteristic. You must use only one of the two currently supported descriptor types: CBUUIDCharacteristicUserDescriptionString or CBUUIDCharacteristicFormatString. For more details about these descriptor types, see CBUUID.

`value`  

The descriptor value to cache. You must provide a non-`nil` value. Once published, you can’t update the value dynamically.

## Return Value

A newly initialized mutable descriptor.

## Discussion

The value type of `value` depends on the type of descriptor:

- The value type of CBUUIDCharacteristicUserDescriptionString is a string you use to provide a human-readable description of the characteristic’s value.

- The value type of a CBUUIDCharacteristicFormatString is an NSData object that you use to specify how to format the characteristic’s value for presentation purposes.

If you want to create a local characteristic format descriptor, the descriptor’s value must conform to the attribute value of the characteristic format descriptor as defined in the Bluetooth 4.0 specification, Volume 3, Part G, Section 3.3.3.5.

For more information, see Core Bluetooth Programming Guide.

