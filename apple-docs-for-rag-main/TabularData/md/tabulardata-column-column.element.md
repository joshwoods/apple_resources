

- TabularData
- Column
-  Column.Element 

Type Alias

# Column.Element

The type of the column’s elements, which is an optional type of the column’s type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
typealias Element = WrappedElement?
```

## See Also

### Inspecting a Column

var name: String

The name of the column.

var count: Int

The number of elements in the column.

var missingCount: Int

The number of missing elements in the column.

var wrappedElementType: any Any.Type

The underlying type of the column’s elements.

