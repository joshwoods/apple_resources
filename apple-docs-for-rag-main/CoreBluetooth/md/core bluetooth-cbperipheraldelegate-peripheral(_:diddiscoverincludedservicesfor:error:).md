

- Core Bluetooth
- CBPeripheralDelegate
-  peripheral(\_:didDiscoverIncludedServicesFor:error:) 

Instance Method

# peripheral(\_:didDiscoverIncludedServicesFor:error:)

Tells the delegate that discovering included services within the indicated service completed.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheral(
    _ peripheral: CBPeripheral,
    didDiscoverIncludedServicesFor service: CBService,
    error: (any Error)?
)
```

## Parameters 

`peripheral`  

The peripheral providing this information.

`service`  

The CBService object containing the included service.

`error`  

The reason the call failed, or `nil` if no error occurred.

## Discussion

Core Bluetooth invokes this method when your app calls the discoverIncludedServices(_:for:) method. If the peripheral successfully discovers services, you can access them through the service’s includedServices property. If successful, the `error` parameter is `nil`. If unsuccessful, the `error` parameter returns the cause of the failure.

## See Also

### Discovering Services

func peripheral(CBPeripheral, didDiscoverServices: (any Error)?)

Tells the delegate that peripheral service discovery succeeded.

