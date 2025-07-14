

- Swift
- RangeReplaceableCollection
-  init(\_:) 

Initializer

# init(\_:)

Creates a new instance of a collection containing the elements of a sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ elements: S) where S : Sequence, Self.Element == S.Element
```

**Required** Default implementation provided.

## Parameters 

`elements`  

The sequence of elements for the new collection. `elements` must be finite.

## Default Implementations

### RangeReplaceableCollection Implementations

init&lt;S>(S)

Creates a new instance of a collection containing the elements of a sequence.

