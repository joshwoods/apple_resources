

- Core Services
- Apple Events
-  AETransactionID 

Type Alias

# AETransactionID

Specifies a transaction ID.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AETransactionID = Int32
```

## Discussion

A transaction is a sequence of Apple events that are sent back and forth between the client and server applications, beginning with the client’s initial request for a service. When you call the AECreateAppleEvent(_:_:_:_:_:_:) function, you pass a value of type `AETransactionID` for the `transactionID` parameter. ID Constants for the AECreateAppleEvent Function lists the valid constant values for a variable or parameter of this type.

