

- Core Bluetooth
- CBPeripheralManagerDelegate
-  peripheralManager(\_:didPublishL2CAPChannel:error:) 

Instance Method

# peripheralManager(\_:didPublishL2CAPChannel:error:)

Tells the delegate that the peripheral manager created a listener for incoming L2CAP channel connections.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheralManager(
    _ peripheral: CBPeripheralManager,
    didPublishL2CAPChannel PSM: CBL2CAPPSM,
    error: (any Error)?
)
```

## Parameters 

`peripheral`  

The peripheral manager that published the channel.

`PSM`  

The Protocol/Service Multiplexer (PSM) of the published channel.

`error`  

The error that prevented publishing, or `nil` if no error occurred.

## Discussion

The peripheral manager calls this method after you call publishL2CAPChannel(withEncryption:). The `PSM` parameter contains the PSM assigned for the published channel.

## See Also

### Using L2CAP Channels

func peripheralManager(CBPeripheralManager, didUnpublishL2CAPChannel: CBL2CAPPSM, error: (any Error)?)

Tells the delegate that the peripheral manager removed a published service from the local system.

func peripheralManager(CBPeripheralManager, didOpen: CBL2CAPChannel?, error: (any Error)?)

Tells the delegate that the peripheral manager opened an L2CAP channel.

