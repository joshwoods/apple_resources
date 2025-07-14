

- Objective-C Runtime
-  objc_setEnumerationMutationHandler(\_:) 

Function

# objc_setEnumerationMutationHandler(\_:)

Sets the current mutation handler.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_setEnumerationMutationHandler(_ handler: ((Any) -> Void)?)
```

## Parameters 

`handler`  

A function pointer to the new mutation handler.

## See Also

### Using Objective-C Language Features

func objc_enumerationMutation(Any)

Inserted by the compiler when a mutation is detected during a foreach iteration.

func imp_implementationWithBlock(Any) -> IMP

Creates a pointer to a function that calls the specified block when the method is called.

func imp_getBlock(IMP) -> Any?

Returns the block associated with an `IMP` that was created using imp_implementationWithBlock(_:).

func imp_removeBlock(IMP) -> Bool

Disassociates a block from an `IMP` that was created using imp_implementationWithBlock(_:), and releases the copy of the block that was created.

func objc_loadWeak(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>) -> Any?

Loads the object referenced by a weak pointer and returns it.

func objc_storeWeak(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, Any?) -> Any?

Stores a new value in a `__weak` variable.

