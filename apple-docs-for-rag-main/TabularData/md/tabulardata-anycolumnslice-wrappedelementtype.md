

- TabularData
- AnyColumnSlice
-  wrappedElementType 

Instance Property

# wrappedElementType

The underlying type of the column’s elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var wrappedElementType: any Any.Type { get }
```

## See Also

### Inspecting a Type-Erased Column Slice

var name: String

The name of the slice’s parent column.

var count: Int

The number of elements in the column slice.

var missingCount: Int

The number of missing elements in the column slice.

func isNil(at: Int) -> Bool

Returns a Boolean that indicates whether the element at the index is missing.

