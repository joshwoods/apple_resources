

- Objective-C Runtime
-  sel_isEqual(\_:\_:) 

Function

# sel_isEqual(\_:\_:)

Returns a Boolean value that indicates whether two selectors are equal.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func sel_isEqual(
    _ lhs: Selector,
    _ rhs: Selector
) -> Bool
```

## Parameters 

`lhs`  

The selector to compare with `rhs`.

`rhs`  

The selector to compare with `lhs`.

## Return Value

YES if `rhs` and `rhs` are equal, otherwise NO.

## Discussion

`sel_isEqual` is equivalent to `==`.

## See Also

### Working with Selectors

func sel_getName(Selector) -> UnsafePointer&lt;CChar>

Returns the name of the method specified by a given selector.

func sel_registerName(UnsafePointer&lt;CChar>) -> Selector

Registers a method with the Objective-C runtime system, maps the method name to a selector, and returns the selector value.

func sel_getUid(UnsafePointer&lt;CChar>) -> Selector

Registers a method name with the Objective-C runtime system.

