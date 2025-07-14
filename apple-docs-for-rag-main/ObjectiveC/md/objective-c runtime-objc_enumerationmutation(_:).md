

- Objective-C Runtime
-  objc_enumerationMutation(\_:) 

Function

# objc_enumerationMutation(\_:)

Inserted by the compiler when a mutation is detected during a foreach iteration.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_enumerationMutation(_ obj: Any)
```

## Parameters 

`obj`  

The object being mutated.

## Discussion

The compiler inserts this function when it detects that an object is mutated during a foreach iteration. The function is called when a mutation occurs, and the enumeration mutation handler is enacted if it is set up (via the objc_setEnumerationMutationHandler(_:) function). If the handler is not set up, a fatal error occurs.

## See Also

### Using Objective-C Language Features

func objc_setEnumerationMutationHandler(((Any) -> Void)?)

Sets the current mutation handler.

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

