

- Swift
-  withUnsafePointer(to:\_:) 

Function

# withUnsafePointer(to:\_:)

Invokes the given closure with a pointer to the given argument.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func withUnsafePointer(
    to value: inout T,
    _ body: (UnsafePointer) throws(E) -> Result
) throws(E) -> Result where E : Error, T : ~Copyable, Result : ~Copyable
```

## Parameters 

`value`  

An instance to temporarily use via pointer. Note that the `inout` exclusivity rules mean that, like any other `inout` argument, `value` cannot be directly accessed by other code for the duration of `body`. Access must only occur through the pointer argument to `body` until `body` returns.

`body`  

A closure that takes a pointer to `value` as its sole argument. If the closure has a return value, that value is also used as the return value of the `withUnsafePointer(to:_:)` function. The pointer argument is valid only for the duration of the function’s execution. It is undefined behavior to try to mutate through the pointer argument by converting it to `UnsafeMutablePointer` or any other mutable pointer type. If you need to mutate the argument through the pointer, use `withUnsafeMutablePointer(to:_:)` instead.

## Return Value

The return value, if any, of the `body` closure.

## Discussion

The `withUnsafePointer(to:_:)` function is useful for calling Objective-C APIs that take in parameters by const pointer.

The pointer argument to `body` is valid only during the execution of `withUnsafePointer(to:_:)`. Do not store or return the pointer for later use.

## See Also

### Pointers to Values

func withUnsafePointer&lt;T, E, Result>(to: borrowing T, (UnsafePointer&lt;T>) throws(E) -> Result) throws(E) -> Result

Invokes the given closure with a pointer to the given argument.

func withUnsafeMutablePointer&lt;T, E, Result>(to: inout T, (UnsafeMutablePointer&lt;T>) throws(E) -> Result) throws(E) -> Result

Calls the given closure with a mutable pointer to the given argument.

func withUnsafeBytes&lt;T, E, Result>(of: inout T, (UnsafeRawBufferPointer) throws(E) -> Result) throws(E) -> Result

Invokes the given closure with a buffer pointer covering the raw bytes of the given argument.

func withUnsafeBytes&lt;T, E, Result>(of: borrowing T, (UnsafeRawBufferPointer) throws(E) -> Result) throws(E) -> Result

Invokes the given closure with a buffer pointer covering the raw bytes of the given argument.

func withUnsafeMutableBytes&lt;T, E, Result>(of: inout T, (UnsafeMutableRawBufferPointer) throws(E) -> Result) throws(E) -> Result

Invokes the given closure with a mutable buffer pointer covering the raw bytes of the given argument.

