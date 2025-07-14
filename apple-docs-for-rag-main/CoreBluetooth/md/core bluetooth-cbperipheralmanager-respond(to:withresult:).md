

- Core Bluetooth
- CBPeripheralManager
-  respond(to:withResult:) 

Instance Method

# respond(to:withResult:)

Responds to a read or write request from a connected central.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func respond(
    to request: CBATTRequest,
    withResult result: CBATTError.Code
)
```

## Parameters 

`request`  

The read or write request received from the connected central. For more information about read and write requests, see CBATTRequest.

`result`  

The result of attempting to fulfill the request. For a list of possible results, see Deprecated Constants.

## Discussion

When the peripheral manager receives a request from a connected central to read or write a characteristic’s value, it calls the peripheralManager(_:didReceiveRead:) or peripheralManager(_:didReceiveWrite:) method of its delegate object. To respond to the corresponding read or write request, you call this method whenever you recevie one of these delegate method callbacks.

