

- RealityKit
- Entity
- Entity.ChildCollection
-  Entity.ChildCollection.SubSequence 

Type Alias

# Entity.ChildCollection.SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
typealias SubSequence = Slice
```

## Discussion

The default subsequence type for collections that don’t define their own is `Slice`.

