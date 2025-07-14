

- Core Bluetooth
- CBPeripheralManager
-  unpublishL2CAPChannel(\_:) 

Instance Method

# unpublishL2CAPChannel(\_:)

Removes a published service from the local system.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.14+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func unpublishL2CAPChannel(_ PSM: CBL2CAPPSM)
```

## Parameters 

`PSM`  

The Protocol and Service Multiplexer (PSM) to remove from the system.

## Discussion

After you make this call, the peripheral manager accepts no new connections for this PSM, and closes any existing L2CAP channels using this PSM.

## See Also

### Using L2CAP Channels

func publishL2CAPChannel(withEncryption: Bool)

Creates a listener for incoming L2CAP channel connections.

