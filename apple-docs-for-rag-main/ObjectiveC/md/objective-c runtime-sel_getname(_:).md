

- Objective-C Runtime
-  sel_getName(\_:) 

Function

# sel_getName(\_:)

Returns the name of the method specified by a given selector.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func sel_getName(_ sel: Selector) -> UnsafePointer
```

## Parameters 

`sel`  

A pointer of type SEL. Pass the selector whose name you wish to determine.

## Return Value

A C string indicating the name of the selector.

## See Also

### Working with Selectors

func sel_registerName(UnsafePointer&lt;CChar>) -> Selector

Registers a method with the Objective-C runtime system, maps the method name to a selector, and returns the selector value.

func sel_getUid(UnsafePointer&lt;CChar>) -> Selector

Registers a method name with the Objective-C runtime system.

func sel_isEqual(Selector, Selector) -> Bool

Returns a Boolean value that indicates whether two selectors are equal.

