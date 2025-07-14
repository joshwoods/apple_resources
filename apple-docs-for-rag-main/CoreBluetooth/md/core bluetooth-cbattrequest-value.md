

- Core Bluetooth
- CBATTRequest
-  value 

Instance Property

# value

The data that the central reads from or writes to the peripheral.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var value: Data? { get set }
```

## Discussion

The value of this property depends on whether the request type is read or write. For read requests, the property is `nil,` and you should set it before responding to the remote central through the respond(to:withResult:) method. For write requests, the value is the data to write to the characteristic’s value.

## See Also

### Requesting to Read and Write Characteristic Values

var central: CBCentral

The remote central device that originated the request.

var characteristic: CBCharacteristic

The characteristic to read or write the value of.

var offset: Int

The zero-based index of the first byte for the read or write request.

