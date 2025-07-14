

- Swift
- CheckedContinuation
-  init(continuation:function:) 

Initializer

# init(continuation:function:)

Creates a checked continuation from an unsafe continuation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    continuation: UnsafeContinuation,
    function: String = #function
)
```

## Parameters 

`continuation`  

An instance of `UnsafeContinuation` that hasn’t yet been resumed. After passing the unsafe continuation to this initializer, don’t use it outside of this object.

`function`  

A string identifying the declaration that is the notional source for the continuation, used to identify the continuation in runtime diagnostics related to misuse of this continuation.

## Discussion

Instead of calling this initializer, most code calls the `withCheckedContinuation(function:_:)` or `withCheckedThrowingContinuation(function:_:)` function instead. You only need to initialize your own `CheckedContinuation` if you already have an `UnsafeContinuation` you want to impose checking on.

