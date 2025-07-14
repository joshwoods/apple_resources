

- Objective-C Runtime
-  method_getImplementation(\_:) 

Function

# method_getImplementation(\_:)

Returns the implementation of a method.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func method_getImplementation(_ m: Method) -> IMP
```

## Parameters 

`m`  

The method to inspect.

## Return Value

A function pointer of type `IMP`.

## See Also

### Working with Methods

func method_getName(Method) -> Selector

Returns the name of a method.

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

func method_getDescription(Method) -> UnsafeMutablePointer&lt;objc_method_description>

Returns a method description structure for a specified method.

func method_setImplementation(Method, IMP) -> IMP

Sets the implementation of a method.

func method_exchangeImplementations(Method, Method)

Exchanges the implementations of two methods.

