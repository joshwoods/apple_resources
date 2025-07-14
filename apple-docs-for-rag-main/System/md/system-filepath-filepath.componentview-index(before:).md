

- System
- FilePath
- FilePath.ComponentView
-  index(before:) 

Instance Method

# index(before:)

Returns the position immediately before the given index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func index(before i: FilePath.ComponentView.Index) -> FilePath.ComponentView.Index
```

## Parameters 

`i`  

A valid index of the collection. `i` must be greater than `startIndex`.

## Return Value

The index value immediately before `i`.

