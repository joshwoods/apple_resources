

- SwiftData
- FetchResultsCollection
-  FetchResultsCollection.SubSequence 

Type Alias

# FetchResultsCollection.SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
typealias SubSequence = Slice>
```

## Discussion

The default subsequence type for collections that don’t define their own is `Slice`.

