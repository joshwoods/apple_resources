

- Core Bluetooth
- CBMutableService
-  init(type:primary:) 

Initializer

# init(type:primary:)

Creates a newly initialized mutable service specified by UUID and service type.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+

``` source
init(
    type UUID: CBUUID,
    primary isPrimary: Bool
)
```

## Parameters 

`UUID`  

A 128-bit UUID that identifies the service.

`isPrimary`  

A Boolean value that indicates whether the type of service is primary or secondary. If the value is true, the type of service is primary. If the value is false, the type of service is secondary.

## Return Value

A newly initialized mutable service.

## Discussion

For more information, see Core Bluetooth Programming Guide.

