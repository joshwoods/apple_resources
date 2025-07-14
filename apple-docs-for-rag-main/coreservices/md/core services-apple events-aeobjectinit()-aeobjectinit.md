

- Core Services
- Apple Events
-  AEObjectInit() 

Function

# AEObjectInit()

Initializes the Object Support Library.

macOS 10.0+

``` source
func AEObjectInit() -> OSErr
```

## Return Value

A result code. See Result Codes.

## Discussion

You must call this function before calling any of the Apple Event Manager functions that describe or manipulate Apple event objects.

You should call the `AEObjectInit` function to initialize the Apple Event Manager functions that handle object specifiers and Apple event objects.

### Version-Notes

To make these functions available to your application with version 1.01 and earlier versions of the Apple Event Manager, you must also link the Apple Event Object Support Library with your application when you build it. For more information, see the Version Notes section for the AppleScript Gestalt Selector described in *Inside macOS: Gestalt Manager Reference* and the function AERemoveSpecialHandler(_:_:_:).

## See Also

### Initializing the Object Support Library

func AESetObjectCallbacks(OSLCompareUPP!, OSLCountUPP!, OSLDisposeTokenUPP!, OSLGetMarkTokenUPP!, OSLMarkUPP!, OSLAdjustMarksUPP!, OSLGetErrDescUPP!) -> OSErr

Specifies the object callback functions for your application.

