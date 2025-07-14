

- Swift
- Dictionary
- Dictionary.Values
-  Dictionary.Values.SubSequence 

Type Alias

# Dictionary.Values.SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias SubSequence = Slice.Values>
```

## Discussion

The default subsequence type for collections that don’t define their own is `Slice`.

