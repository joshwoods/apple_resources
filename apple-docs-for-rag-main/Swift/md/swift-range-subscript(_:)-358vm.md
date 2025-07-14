

- Swift
- Range
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the subsequence bounded by the given range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(bounds: Range.Index>) -> Range { get }
```

Available when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

## Parameters 

`bounds`  

A range of the range’s indices. The upper and lower bounds of the `bounds` range must be valid indices of the collection.

