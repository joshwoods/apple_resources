

- Nearby Interaction
- NINearbyAccessoryConfiguration
-  init(accessoryData:bluetoothPeerIdentifier:) 

Initializer

# init(accessoryData:bluetoothPeerIdentifier:)

Creates a configuration for an accessory with the given Bluetooth peer identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
init(
    accessoryData: Data,
    bluetoothPeerIdentifier identifier: UUID
) throws
```

## Parameters 

`accessoryData`  

The accessory’s configuration data formatted to the Ultra Wideband (UWB) third-party device specification.

`identifier`  

The accessory’s Bluetooth peer identifier. For more information, see CBPeer identifier.

## Mentioned in 

Initiating and maintaining a session

## Discussion

Use this initializer when your app interacts with a Bluetooth accessory that’s paired to the device to enable interaction while your app is in the background.

## See Also

### Creating a configuration

init(data: Data) throws

Creates a configuration for interaction between iPhone and third-party accessories.

