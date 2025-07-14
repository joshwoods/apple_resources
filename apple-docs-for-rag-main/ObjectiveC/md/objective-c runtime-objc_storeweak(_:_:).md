

- Objective-C Runtime
-  objc_storeWeak(\_:\_:) 

Function

# objc_storeWeak(\_:\_:)

Stores a new value in a `__weak` variable.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func objc_storeWeak(
    _ location: AutoreleasingUnsafeMutablePointer,
    _ obj: Any?
) -> Any?
```

## Parameters 

`location`  

The address of the weak pointer.

`obj`  

The new object you want the weak pointer to now point to.

## Return Value

The value stored in `location` (that is, `obj`).

## Discussion

This function is typically used anywhere a `__weak` variable is the target of an assignment.

## See Also

### Using Objective-C Language Features

func objc_enumerationMutation(Any)

Inserted by the compiler when a mutation is detected during a foreach iteration.

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

