

- Core Bluetooth
- CBATTRequest
-  characteristic 

Instance Property

# characteristic

The characteristic to read or write the value of.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var characteristic: CBCharacteristic { get }
```

## See Also

### Requesting to Read and Write Characteristic Values

var central: CBCentral

The remote central device that originated the request.

var value: Data?

The data that the central reads from or writes to the peripheral.

var offset: Int

The zero-based index of the first byte for the read or write request.

