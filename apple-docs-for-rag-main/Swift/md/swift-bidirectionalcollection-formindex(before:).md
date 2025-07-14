

- Swift
- BidirectionalCollection
-  formIndex(before:) 

Instance Method

# formIndex(before:)

Replaces the given index with its predecessor.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func formIndex(before i: inout Self.Index)
```

**Required** Default implementation provided.

## Parameters 

`i`  

A valid index of the collection. `i` must be greater than `startIndex`.

## Default Implementations

### BidirectionalCollection Implementations

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

