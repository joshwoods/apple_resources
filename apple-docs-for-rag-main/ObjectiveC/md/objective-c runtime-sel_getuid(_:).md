

- Objective-C Runtime
-  sel_getUid(\_:) 

Function

# sel_getUid(\_:)

Registers a method name with the Objective-C runtime system.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func sel_getUid(_ str: UnsafePointer) -> Selector
```

## Parameters 

`str`  

A pointer to a C string. Pass the name of the method you wish to register.

## Return Value

A pointer of type SEL specifying the selector for the named method.

## Discussion

The implementation of this method is identical to the implementation of sel_registerName(_:).

### Version-Notes

Prior to OS X version 10.0, this method tried to find the selector mapped to the given name and returned `NULL` if the selector was not found. This was changed for safety, because it was observed that many of the callers of this function did not check the return value for `NULL`.

## See Also

### Working with Selectors

func sel_getName(Selector) -> UnsafePointer&lt;CChar>

Returns the name of the method specified by a given selector.

func sel_registerName(UnsafePointer&lt;CChar>) -> Selector

Registers a method with the Objective-C runtime system, maps the method name to a selector, and returns the selector value.

func sel_isEqual(Selector, Selector) -> Bool

Returns a Boolean value that indicates whether two selectors are equal.

