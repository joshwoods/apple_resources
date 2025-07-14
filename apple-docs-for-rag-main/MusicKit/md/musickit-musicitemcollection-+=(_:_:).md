

- MusicKit
- MusicItemCollection
-  +=(\_:\_:) 

Operator

# +=(\_:\_:)

Appends contents of a collection representing a next batch, in the right hand side, to the existing collection on the left hand side.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func += (collection: inout MusicItemCollection, nextBatchCollection: MusicItemCollection)
```

## Discussion

In addition to appending the underlying items of the collection to the existing collection on the left hand side, this will also transfer to the collection on the left hand side any information about a next batch from the collection on the right hand side, or lack thereof.

This appending operator is particularly useful for aggregating subsequent batches from a given collection into a local variable (for example, to use a MusicItemCollection to drive a SwiftUI List or ForEach).

