

- SwiftUI
- ViewSpacing
-  union(\_:edges:) 

Instance Method

# union(\_:edges:)

Gets a new value that merges the spacing preferences of another spacing instance with this instance for a specified set of edges.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func union(
    _ other: ViewSpacing,
    edges: Edge.Set = .all
) -> ViewSpacing
```

## Parameters 

`other`  

Another spacing preferences instance to merge with this one.

`edges`  

The edges to merge. Edges that you don’t specify are unchanged after the method completes.

## Return Value

A new view spacing preferences instance with the merged values.

## Discussion

This method behaves like formUnion(_:edges:), except that it creates a copy of the original spacing preferences instance before merging, leaving the original instance unmodified.

## See Also

### Merging spacing instances

func formUnion(ViewSpacing, edges: Edge.Set)

Merges the spacing preferences of another spacing instance with this instance for a specified set of edges.

