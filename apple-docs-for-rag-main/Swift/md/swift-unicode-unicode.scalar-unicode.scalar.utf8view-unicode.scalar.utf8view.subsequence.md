

- Swift
- Unicode
- Unicode.Scalar
- Unicode.Scalar.UTF8View
-  Unicode.Scalar.UTF8View.SubSequence 

Type Alias

# Unicode.Scalar.UTF8View.SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias SubSequence = Slice
```

## Discussion

The default subsequence type for collections that don’t define their own is `Slice`.

