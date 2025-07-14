

- Core Bluetooth
- CBCentral
-  maximumUpdateValueLength 

Instance Property

# maximumUpdateValueLength

The maximum amount of data, in bytes, that the central can receive in a single notification or indication.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var maximumUpdateValueLength: Int { get }
```

## Topics

### Related Documentation

func updateValue(Data, for: CBMutableCharacteristic, onSubscribedCentrals: [CBCentral]?) -> Bool

Send an updated characteristic value to one or more subscribed centrals, using a notification or indication.

