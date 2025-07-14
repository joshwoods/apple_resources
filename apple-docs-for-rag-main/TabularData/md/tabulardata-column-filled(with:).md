

- TabularData
- Column
-  filled(with:) 

Instance Method

# filled(with:)

Generates a filled column by replacing missing elements with a value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func filled(with value: Self.WrappedElement) -> FilledColumn
```

## Parameters 

`value`  

A value the method uses to replace the column’s missing elements.

## Return Value

A filled column.

## See Also

### Creating Transformed Columns

func map&lt;T>((Column&lt;WrappedElement>.Element) throws -> T?) rethrows -> Column&lt;T>

Creates a new column by applying a transformation to every element.

func mapNonNil&lt;T>((WrappedElement) throws -> T?) rethrows -> Column&lt;T>

Creates a new column by applying the transformation to every element that isn’t missing.

