

- TabularData
- AnyColumnSlice
-  count 

Instance Property

# count

The number of elements in the column slice.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var count: Int { get }
```

## See Also

### Inspecting a Type-Erased Column Slice

var name: String

The name of the slice’s parent column.

var missingCount: Int

The number of missing elements in the column slice.

var wrappedElementType: any Any.Type

The underlying type of the column’s elements.

func isNil(at: Int) -> Bool

Returns a Boolean that indicates whether the element at the index is missing.

