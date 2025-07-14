

- Objective-C Runtime
-  imp_implementationWithBlock(\_:) 

Function

# imp_implementationWithBlock(\_:)

Creates a pointer to a function that calls the specified block when the method is called.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func imp_implementationWithBlock(_ block: Any) -> IMP
```

## Parameters 

`block`  

The block that implements this method. The signature of `block` should be `method_return_type ^(id self, method_args …)`. The selector of the method is not available to `block`. `block` is copied with `Block_copy()`.

## Return Value

The IMP that calls `block`. You must dispose of the returned IMP using the function.

## See Also

### Using Objective-C Language Features

func objc_enumerationMutation(Any)

Inserted by the compiler when a mutation is detected during a foreach iteration.

func objc_setEnumerationMutationHandler(((Any) -> Void)?)

Sets the current mutation handler.

func imp_getBlock(IMP) -> Any?

Returns the block associated with an `IMP` that was created using imp_implementationWithBlock(_:).

func imp_removeBlock(IMP) -> Bool

Disassociates a block from an `IMP` that was created using imp_implementationWithBlock(_:), and releases the copy of the block that was created.

func objc_loadWeak(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>) -> Any?

Loads the object referenced by a weak pointer and returns it.

func objc_storeWeak(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>, Any?) -> Any?

Stores a new value in a `__weak` variable.

