

- Swift
- ClosedRange
-  init(\_:) 

Initializer

# init(\_:)

Now that Range is conditionally a collection when Bound: Strideable, CountableRange is no longer needed. This is a deprecated initializer for any remaining uses of Range(countableRange).

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ other: ClosedRange)
```

Available when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

