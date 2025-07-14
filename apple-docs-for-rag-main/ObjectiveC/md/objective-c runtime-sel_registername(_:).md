

- Objective-C Runtime
-  sel_registerName(\_:) 

Function

# sel_registerName(\_:)

Registers a method with the Objective-C runtime system, maps the method name to a selector, and returns the selector value.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func sel_registerName(_ str: UnsafePointer) -> Selector
```

## Parameters 

`str`  

A pointer to a C string. Pass the name of the method you wish to register.

## Return Value

A pointer of type SEL specifying the selector for the named method.

## Discussion

You must register a method name with the Objective-C runtime system to obtain the method’s selector before you can add the method to a class definition. If the method name has already been registered, this function simply returns the selector.

## See Also

### Working with Selectors

func sel_getName(Selector) -> UnsafePointer&lt;CChar>

Returns the name of the method specified by a given selector.

func sel_getUid(UnsafePointer&lt;CChar>) -> Selector

Registers a method name with the Objective-C runtime system.

func sel_isEqual(Selector, Selector) -> Bool

Returns a Boolean value that indicates whether two selectors are equal.

