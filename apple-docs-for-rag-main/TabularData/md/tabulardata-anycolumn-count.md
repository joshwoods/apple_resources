

- TabularData
- AnyColumn
-  count 

Instance Property

# count

The number of elements in the column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var count: Int { get }
```

## See Also

### Inspecting a Type-Erased Column

var name: String

The name of the column.

var missingCount: Int

The number of missing elements in the column.

var wrappedElementType: any Any.Type

The underlying type of the column’s elements.

func isNil(at: Int) -> Bool

Returns a Boolean that indicates whether the element at the index is missing.

