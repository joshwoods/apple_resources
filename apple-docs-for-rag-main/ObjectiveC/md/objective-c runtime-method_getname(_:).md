

- Objective-C Runtime
-  method_getName(\_:) 

Function

# method_getName(\_:)

Returns the name of a method.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func method_getName(_ m: Method) -> Selector
```

## Parameters 

`m`  

The method to inspect.

## Return Value

A pointer of type SEL.

## Discussion

To get the method name as a C string, call `sel_getName(method_getName(method))`.

## See Also

### Working with Methods

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

func method_getDescription(Method) -> UnsafeMutablePointer&lt;objc_method_description>

Returns a method description structure for a specified method.

func method_setImplementation(Method, IMP) -> IMP

Sets the implementation of a method.

func method_exchangeImplementations(Method, Method)

Exchanges the implementations of two methods.

