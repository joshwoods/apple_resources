

- Core Services
- Carbon Core
- Carbon Core Functions
-  NewOSLCompareUPP(\_:) 

Function

# NewOSLCompareUPP(\_:)

Creates a new universal procedure pointer to an object callback comparison function.

macOS 10.0+

``` source
func NewOSLCompareUPP(_ userRoutine: OSLCompareProcPtr!) -> OSLCompareUPP!
```

## Return Value

See OSLCompareUPP.

## Discussion

See the OSLCompareProcPtr callback function.

## See Also

### Creating, Calling, and Deleting Universal Procedure Pointers

func DisposeAECoerceDescUPP(AECoerceDescUPP!)

Disposes of a universal procedure pointer to a function that coerces data stored in a descriptor.

func DisposeAECoercePtrUPP(AECoercePtrUPP!)

Disposes of a universal procedure pointer to a function that coerces data stored in a buffer.

func DisposeAEDisposeExternalUPP(AEDisposeExternalUPP!)

Disposes of a universal procedure pointer to a function that disposes of data supplied to the `AECreateDescFromExternalPtr` function.

func DisposeAEEventHandlerUPP(AEEventHandlerUPP!)

Disposes of a universal procedure pointer to an event handler function.

func DisposeOSLAccessorUPP(OSLAccessorUPP!)

Disposes of a universal procedure pointer to an object accessor function.

func DisposeOSLAdjustMarksUPP(OSLAdjustMarksUPP!)

Disposes of a universal procedure pointer to an object callback adjust marks function.

func DisposeOSLCompareUPP(OSLCompareUPP!)

Disposes of a universal procedure pointer to an object callback comparison function.

func DisposeOSLCountUPP(OSLCountUPP!)

Disposes of a universal procedure pointer to an object callback count function.

func DisposeOSLDisposeTokenUPP(OSLDisposeTokenUPP!)

Disposes of a universal procedure pointer to an object callback dispose token function.

func DisposeOSLGetErrDescUPP(OSLGetErrDescUPP!)

Disposes of a universal procedure pointer to an object callback get error descriptor function.

func DisposeOSLGetMarkTokenUPP(OSLGetMarkTokenUPP!)

Disposes of a universal procedure pointer to an object callback get mark function.

func DisposeOSLMarkUPP(OSLMarkUPP!)

Disposes of a universal procedure pointer to an object callback mark function.

func InvokeAECoerceDescUPP(UnsafePointer&lt;AEDesc>!, DescType, SRefCon!, UnsafeMutablePointer&lt;AEDesc>!, AECoerceDescUPP!) -> OSErr

Calls a universal procedure pointer to a function that coerces data stored in a descriptor.

func InvokeAECoercePtrUPP(DescType, UnsafeRawPointer!, Size, DescType, SRefCon!, UnsafeMutablePointer&lt;AEDesc>!, AECoercePtrUPP!) -> OSErr

Calls a universal procedure pointer to a function that coerces data stored in a buffer.

func InvokeAEDisposeExternalUPP(UnsafeRawPointer!, Size, SRefCon!, AEDisposeExternalUPP!)

Calls a dispose external universal procedure pointer.

func InvokeAEEventHandlerUPP(UnsafePointer&lt;AppleEvent>!, UnsafeMutablePointer&lt;AppleEvent>!, SRefCon!, AEEventHandlerUPP!) -> OSErr

Calls an event handler universal procedure pointer.

func InvokeOSLAccessorUPP(DescType, UnsafePointer&lt;AEDesc>!, DescType, DescType, UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;AEDesc>!, SRefCon!, OSLAccessorUPP!) -> OSErr

Calls an object accessor universal procedure pointer.

func InvokeOSLAdjustMarksUPP(Int, Int, UnsafePointer&lt;AEDesc>!, OSLAdjustMarksUPP!) -> OSErr

Calls an object callback adjust marks universal procedure pointer.

func InvokeOSLCompareUPP(DescType, UnsafePointer&lt;AEDesc>!, UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;DarwinBoolean>!, OSLCompareUPP!) -> OSErr

Calls an object callback comparison universal procedure pointer.

func InvokeOSLCountUPP(DescType, DescType, UnsafePointer&lt;AEDesc>!, UnsafeMutablePointer&lt;Int>!, OSLCountUPP!) -> OSErr

Calls an object callback count universal procedure pointer.

func InvokeOSLDisposeTokenUPP(UnsafeMutablePointer&lt;AEDesc>!, OSLDisposeTokenUPP!) -> OSErr

Calls an object callback dispose token universal procedure pointer.

func InvokeOSLGetErrDescUPP(UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;AEDesc>?>!, OSLGetErrDescUPP!) -> OSErr

Calls an object callback get error descriptor universal procedure pointer.

func InvokeOSLGetMarkTokenUPP(UnsafePointer&lt;AEDesc>!, DescType, UnsafeMutablePointer&lt;AEDesc>!, OSLGetMarkTokenUPP!) -> OSErr

Calls an object callback get mark universal procedure pointer.

func InvokeOSLMarkUPP(UnsafePointer&lt;AEDesc>!, UnsafePointer&lt;AEDesc>!, Int, OSLMarkUPP!) -> OSErr

Calls an object callback mark universal procedure pointer.

func NewAECoerceDescUPP(AECoerceDescProcPtr!) -> AECoerceDescUPP!

Creates a new universal procedure pointer to a function that coerces data stored in a descriptor.

func NewAECoercePtrUPP(AECoercePtrProcPtr!) -> AECoercePtrUPP!

Creates a new universal procedure pointer to a function that coerces data stored in a buffer.

func NewAEDisposeExternalUPP(AEDisposeExternalProcPtr!) -> AEDisposeExternalUPP!

Creates a new universal procedure pointer to a function that disposes of data stored in a buffer.

func NewAEEventHandlerUPP(AEEventHandlerProcPtr!) -> AEEventHandlerUPP!

Creates a new universal procedure pointer to an event handler function.

func NewOSLAccessorUPP(OSLAccessorProcPtr!) -> OSLAccessorUPP!

Creates a new universal procedure pointer to an object accessor function.

func NewOSLAdjustMarksUPP(OSLAdjustMarksProcPtr!) -> OSLAdjustMarksUPP!

Creates a new universal procedure pointer to an object callback adjust marks function.

func NewOSLCountUPP(OSLCountProcPtr!) -> OSLCountUPP!

Creates a new universal procedure pointer to an object callback count function.

func NewOSLDisposeTokenUPP(OSLDisposeTokenProcPtr!) -> OSLDisposeTokenUPP!

Creates a new universal procedure pointer to an object callback dispose token function.

func NewOSLGetErrDescUPP(OSLGetErrDescProcPtr!) -> OSLGetErrDescUPP!

Creates a new universal procedure pointer to an object callback get error descriptor function.

func NewOSLGetMarkTokenUPP(OSLGetMarkTokenProcPtr!) -> OSLGetMarkTokenUPP!

Creates a new universal procedure pointer to an object callback get mark function.

func NewOSLMarkUPP(OSLMarkProcPtr!) -> OSLMarkUPP!

Creates a new universal procedure pointer to an object callback mark function.

