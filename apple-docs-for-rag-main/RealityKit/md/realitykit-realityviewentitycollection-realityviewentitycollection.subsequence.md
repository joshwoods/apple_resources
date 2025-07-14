

- RealityKit
- RealityViewEntityCollection
-  RealityViewEntityCollection.SubSequence 

Type Alias

# RealityViewEntityCollection.SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
typealias SubSequence = Slice
```

## Discussion

The default subsequence type for collections that don’t define their own is `Slice`.

