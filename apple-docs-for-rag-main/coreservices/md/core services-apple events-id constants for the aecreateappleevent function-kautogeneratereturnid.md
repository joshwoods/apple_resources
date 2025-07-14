

- Core Services
- Apple Events
- ID Constants for the AECreateAppleEvent Function
-  kAutoGenerateReturnID 

Global Variable

# kAutoGenerateReturnID

If you pass this value for the `returnID` parameter of the AECreateAppleEvent(_:_:_:_:_:_:) function, the Apple Event Manager assigns to the created Apple event a return ID that is unique to the current session.

Mac Catalyst 13.0+macOS 10.0+

``` source
var kAutoGenerateReturnID: Int { get }
```

