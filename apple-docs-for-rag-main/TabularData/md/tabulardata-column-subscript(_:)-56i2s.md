

- TabularData
- Column
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns a column slice that includes elements that correspond to a collection of Booleans.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(mask: C) -> DiscontiguousColumnSlice where C : Collection, C.Element == Bool { get }
```

## Parameters 

`mask`  

A Boolean collection. The subscript returns a slice that includes the column elements that correspond to the `true` elements in `mask`.

## Overview

You can create a Boolean column for this subscript by comparing a column to a value of the column elements’ type.

```
let followerColumn = artists["Followers", Int.self].filled(with: 0)
let popularArtists = artists[followerColumn > 10_000_000]
```

