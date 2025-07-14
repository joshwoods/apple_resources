

- TabularData
- FilledColumn
-  distance(from:to:) 

Instance Method

# distance(from:to:)

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func distance(
    from start: Self.Index,
    to end: Self.Index
) -> Int
```

## See Also

### Finding an Element Index

func lastIndex(of: Self.Element) -> Self.Index?

Returns the last index where the specified value appears in the collection.

func lastIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the index of the last element in the collection that matches the given predicate.

