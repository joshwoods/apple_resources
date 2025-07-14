

- Core Services
- Apple Events
-  AEReturnID 

Type Alias

# AEReturnID

Specifies a return ID for a created Apple event.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AEReturnID = Int16
```

## Discussion

When you call the AECreateAppleEvent(_:_:_:_:_:_:) function, you pass a value of type `AEReturnID` for the `returnID` parameter. ID Constants for the AECreateAppleEvent Function lists the valid constant values for a variable or parameter of this type.

