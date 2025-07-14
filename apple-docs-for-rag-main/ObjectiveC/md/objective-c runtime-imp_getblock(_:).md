

- Objective-C Runtime
-  imp_getBlock(\_:) 

Function

# imp_getBlock(\_:)

Returns the block associated with an `IMP` that was created using imp_implementationWithBlock(_:).

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func imp_getBlock(_ anImp: IMP) -> Any?
```

## Parameters 

`anImp`  

The IMP that calls this block.

## Return Value

The block called by `anImp`.

## See Also

### Using Objective-C Language Features

func objc_enumerationMutation(Any)

Inserted by the compiler when a mutation is detected during a foreach iteration.

func objc_setEnumerationMutationHandler(((Any) -> Void)?)

Sets the current mutation handler.

func imp_implementationWithBlock(Any) -> IMP

Creates a pointer to a function that calls the specified block when the method is called.

func imp_removeBlock(IMP) -> Bool

Disassociates a block from an `IMP` that was created using imp_implementationWithBlock(_:), and releases the copy of the block that was created.

func objc_loadWeak(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>) -> Any?

Loads the object referenced by a weak pointer and returns it.

func objc_storeWeak(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, Any?) -> Any?

Stores a new value in a `__weak` variable.

