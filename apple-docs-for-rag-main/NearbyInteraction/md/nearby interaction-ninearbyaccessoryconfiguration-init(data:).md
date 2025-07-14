

- Nearby Interaction
- NINearbyAccessoryConfiguration
-  init(data:) 

Initializer

# init(data:)

Creates a configuration for interaction between iPhone and third-party accessories.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+watchOS 8.0+

``` source
init(data: Data) throws
```

## Parameters 

`data`  

The accessory’s configuration data formatted to the Ultra Wideband (UWB) third-party device specification.

## Mentioned in 

Initiating and maintaining a session

## See Also

### Creating a configuration

init(accessoryData: Data, bluetoothPeerIdentifier: UUID) throws

Creates a configuration for an accessory with the given Bluetooth peer identifier.

