

- Swift
- SetAlgebra
-  init(\_:) 

Initializer

# init(\_:)

Creates a new set from a finite sequence of items.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ sequence: S) where S : Sequence, Self.Element == S.Element
```

**Required** Default implementation provided.

## Parameters 

`sequence`  

The elements to use as members of the new set.

## Discussion

Use this initializer to create a new set from an existing sequence, like an array or a range:

```
let validIndices = Set(0..

## Default Implementations

### SetAlgebra Implementations

init&lt;S>(S)

Creates a new set from a finite sequence of items.

