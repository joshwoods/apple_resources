

- Swift
- Range
-  init(\_:) 

Initializer

# init(\_:)

Creates an instance equivalent to the given `ClosedRange`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ other: ClosedRange)
```

Available when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

## Parameters 

`other`  

A closed range to convert to a `Range` instance.

## Discussion

An equivalent range must be representable as an instance of Range. For example, passing a closed range with an upper bound of `Int.max` triggers a runtime error, because the resulting half-open range would require an upper bound of `Int.max + 1`, which is not representable as an `Int`.

