

- Core Bluetooth
- CBPeripheralDelegate
-  peripheral(\_:didDiscoverServices:) 

Instance Method

# peripheral(\_:didDiscoverServices:)

Tells the delegate that peripheral service discovery succeeded.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheral(
    _ peripheral: CBPeripheral,
    didDiscoverServices error: (any Error)?
)
```

## Parameters 

`peripheral`  

The peripheral to which the services belong.

`error`  

The reason the call failed, or `nil` if no error occurred.

## Discussion

Core Bluetooth invokes this method when your app calls the discoverServices(_:) method. If the peripheral successfully discovers services, you can access them through the peripheral’s services property. If successful, the `error` parameter is `nil`. If unsuccessful, the `error` parameter returns the cause of the failure.

For more information, see Core Bluetooth Programming Guide.

## See Also

### Discovering Services

func peripheral(CBPeripheral, didDiscoverIncludedServicesFor: CBService, error: (any Error)?)

Tells the delegate that discovering included services within the indicated service completed.

