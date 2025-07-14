

- Core Bluetooth
- CBATTRequest
-  offset 

Instance Property

# offset

The zero-based index of the first byte for the read or write request.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var offset: Int { get }
```

## Discussion

You can use the value of this property to ensure that the ATT request is attempting to read or write within the proper bounds of the characteristic’s value. For an example of how to take a request’s offset property into account when responding to a read or write request, see Responding to Read and Write Requests from a Central.

## See Also

### Requesting to Read and Write Characteristic Values

var central: CBCentral

The remote central device that originated the request.

var characteristic: CBCharacteristic

The characteristic to read or write the value of.

var value: Data?

The data that the central reads from or writes to the peripheral.

