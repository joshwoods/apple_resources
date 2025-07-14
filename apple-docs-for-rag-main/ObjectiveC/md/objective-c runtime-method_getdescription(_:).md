

- Objective-C Runtime
-  method_getDescription(\_:) 

Function

# method_getDescription(\_:)

Returns a method description structure for a specified method.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func method_getDescription(_ m: Method) -> UnsafeMutablePointer
```

## Parameters 

`m`  

The method you want to inquire about.

## Return Value

An `objc_method_description` structure that describes the method specified by `m`.

## See Also

### Working with Methods

func method_getName(Method) -> Selector

Returns the name of a method.

func method_getImplementation(Method) -> IMP

Returns the implementation of a method.

func method_getTypeEncoding(Method) -> UnsafePointer&lt;CChar>?

Returns a string describing a method’s parameter and return types.

func method_copyReturnType(Method) -> UnsafeMutablePointer&lt;CChar>

Returns a string describing a method’s return type.

func method_copyArgumentType(Method, UInt32) -> UnsafeMutablePointer&lt;CChar>?

Returns a string describing a single parameter type of a method.

func method_getReturnType(Method, UnsafeMutablePointer&lt;CChar>, Int)

Returns by reference a string describing a method’s return type.

func method_getNumberOfArguments(Method) -> UInt32

Returns the number of arguments accepted by a method.

func method_getArgumentType(Method, UInt32, UnsafeMutablePointer&lt;CChar>?, Int)

Returns by reference a string describing a single parameter type of a method.

func method_setImplementation(Method, IMP) -> IMP

Sets the implementation of a method.

func method_exchangeImplementations(Method, Method)

Exchanges the implementations of two methods.

