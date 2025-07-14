

- Core Bluetooth
- CBPeripheralManagerDelegate
-  peripheralManager(\_:didReceiveRead:) 

Instance Method

# peripheralManager(\_:didReceiveRead:)

Tells the delegate that a local peripheral received an Attribute Protocol (ATT) read request for a characteristic with a dynamic value.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func peripheralManager(
    _ peripheral: CBPeripheralManager,
    didReceiveRead request: CBATTRequest
)
```

## Parameters 

`peripheral`  

The peripheral manager that received the request.

`request`  

A CBATTRequest object that represents a request to read a characteristic’s value.

## Discussion

When you receive this callback, call the respond(to:withResult:) method of the CBPeripheralManager class exactly once to respond to the read request.

## See Also

### Receiving Read and Write Requests

func peripheralManager(CBPeripheralManager, didReceiveWrite: [CBATTRequest])

Tells the delegate that a local peripheral device received an Attribute Protocol (ATT) write request for a characteristic with a dynamic value.

