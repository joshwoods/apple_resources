

- MusicKit
- MusicItemCollection
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a contiguous subrange of the collection’s elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(bounds: Range.Index>) -> MusicItemCollection.SubSequence { get }
```

Available when `MusicItemType` conforms to `MusicItem`.

## Parameters 

`bounds`  

A range of the collection’s indices. The bounds of the range must be valid indices of the collection.

## Overview

The accessed slice uses the same indices for the same elements as the original collection uses. Always use the slice’s `startIndex` property instead of assuming that its indices start at a particular value.

This example demonstrates getting a slice of an array of strings, finding the index of one of the strings in the slice, and then using that index in the original array.

```
let streets = ["Adams", "Bryant", "Channing", "Douglas", "Evarts"]
let streetsSlice = streets[2 ..

Complexity

O(1)

