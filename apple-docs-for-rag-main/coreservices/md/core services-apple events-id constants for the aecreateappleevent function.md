

- Core Services
- Apple Events
-  ID Constants for the AECreateAppleEvent Function 

# ID Constants for the AECreateAppleEvent Function

Specify values for the ID parameters of the `AECreateAppleEvent` function.

## Overview

You use these constants with the AECreateAppleEvent(_:_:_:_:_:_:) function.

## Topics

### Constants

var kAutoGenerateReturnID: Int

If you pass this value for the `returnID` parameter of the AECreateAppleEvent(_:_:_:_:_:_:) function, the Apple Event Manager assigns to the created Apple event a return ID that is unique to the current session.

var kAnyTransactionID: Int

