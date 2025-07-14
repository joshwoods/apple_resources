

- TabularData
- ColumnSlice
-  map(\_:) 

Instance Method

# map(\_:)

Creates a new column by applying a transformation to every element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func map(_ transform: (ColumnSlice.Element) throws -> T?) rethrows -> Column
```

## Parameters 

`transform`  

The transformation closure.

## See Also

### Creating Transformed Columns

func filled(with: Self.WrappedElement) -> FilledColumn&lt;Self>

Generates a filled column by replacing missing elements with a value.

