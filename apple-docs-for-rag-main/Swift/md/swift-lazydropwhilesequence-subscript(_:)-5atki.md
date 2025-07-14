

- Swift
- LazyDropWhileSequence
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a view of this collection with the elements at the given indices.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
subscript(subranges: RangeSet) -> DiscontiguousSlice { get }
```

## Parameters 

`subranges`  

The indices of the elements to retrieve from this collection.

## Return Value

A collection of the elements at the positions in `subranges`.

## Overview

Complexity

O(1)

