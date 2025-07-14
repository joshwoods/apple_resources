

- Swift
- ClosedRange
-  init(\_:) 

Initializer

# init(\_:)

Creates an instance equivalent to the given `Range`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ other: Range)
```

Available when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

## Parameters 

`other`  

A `Range` to convert to a `ClosedRange` instance.

## Discussion

An equivalent range must be representable as a closed range. For example, passing an empty range as `other` triggers a runtime error, because an empty range cannot be represented by a closed range instance.

