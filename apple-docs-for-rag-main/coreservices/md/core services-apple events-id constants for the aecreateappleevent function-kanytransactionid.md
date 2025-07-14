

- Core Services
- Apple Events
- ID Constants for the AECreateAppleEvent Function
-  kAnyTransactionID 

Global Variable

# kAnyTransactionID

Mac Catalyst 13.0+macOS 10.0+

``` source
var kAnyTransactionID: Int { get }
```

## Discussion

You pass this value for the `transactionID` parameter of the AECreateAppleEvent(_:_:_:_:_:_:) function if the Apple event is not one of a series of interdependent Apple events.

A transaction is a sequence of Apple events that are sent back and forth between the client and server applications, beginning with the client’s initial request for a service. All Apple events that are part of a transaction must have the same transaction ID.

