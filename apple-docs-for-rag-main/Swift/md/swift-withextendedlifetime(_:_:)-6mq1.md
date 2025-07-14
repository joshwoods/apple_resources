

- Swift
-  withExtendedLifetime(\_:\_:) 

Function

# withExtendedLifetime(\_:\_:)

Evaluates a closure while ensuring that the given instance is not destroyed before the closure returns.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func withExtendedLifetime(
    _ x: borrowing T,
    _ body: () throws(E) -> Result
) throws(E) -> Result where E : Error, T : ~Copyable, Result : ~Copyable
```

## Parameters 

`x`  

An instance to preserve until the execution of `body` is completed.

`body`  

A closure to execute that depends on the lifetime of `x` being extended. If `body` has a return value, that value is also used as the return value for the `withExtendedLifetime(_:_:)` method.

## Return Value

The return value, if any, of the `body` closure parameter.

## See Also

### Reference Counting

struct Unmanaged

A type for propagating an unmanaged object reference.

func withExtendedLifetime&lt;T, E, Result>(borrowing T, (borrowing T) throws(E) -> Result) throws(E) -> Result

Evaluates a closure while ensuring that the given instance is not destroyed before the closure returns.

