

- Core Bluetooth
- CBPeripheralManager
-  publishL2CAPChannel(withEncryption:) 

Instance Method

# publishL2CAPChannel(withEncryption:)

Creates a listener for incoming L2CAP channel connections.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.14+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func publishL2CAPChannel(withEncryption encryptionRequired: Bool)
```

## Parameters 

`encryptionRequired`  

true if the service requires link encryption before a stream can be established. false if the service supports use over an unsecured link.

## Discussion

The system determines an unused Protocol and Service Multiplexer (PSM) at the time of publishing, and provides it to your app with peripheralManager(_:didPublishL2CAPChannel:error:). L2CAP channels aren’t discoverable by themselves, so it’s the app’s responsibility to handle PSM discovery on the client.

## See Also

### Using L2CAP Channels

func unpublishL2CAPChannel(CBL2CAPPSM)

Removes a published service from the local system.

