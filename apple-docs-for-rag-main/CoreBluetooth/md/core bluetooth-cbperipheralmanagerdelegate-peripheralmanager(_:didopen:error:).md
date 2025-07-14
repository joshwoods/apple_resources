

- Core Bluetooth
- CBPeripheralManagerDelegate
-  peripheralManager(\_:didOpen:error:) 

Instance Method

# peripheralManager(\_:didOpen:error:)

Tells the delegate that the peripheral manager opened an L2CAP channel.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional func peripheralManager(
    _ peripheral: CBPeripheralManager,
    didOpen channel: CBL2CAPChannel?,
    error: (any Error)?
)
```

## Parameters 

`peripheral`  

The peripheral manager that opened the channel.

`channel`  

The channel opened by the manager.

`error`  

The error that occurred, or `nil` if no error occurred.

## Discussion

The peripheral manager calls this method after you call publishL2CAPChannel(withEncryption:).

## See Also

### Using L2CAP Channels

func peripheralManager(CBPeripheralManager, didPublishL2CAPChannel: CBL2CAPPSM, error: (any Error)?)

Tells the delegate that the peripheral manager created a listener for incoming L2CAP channel connections.

func peripheralManager(CBPeripheralManager, didUnpublishL2CAPChannel: CBL2CAPPSM, error: (any Error)?)

Tells the delegate that the peripheral manager removed a published service from the local system.

