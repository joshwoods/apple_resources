

- TabularData
- Column
-  mapNonNil(\_:) 

Instance Method

# mapNonNil(\_:)

Creates a new column by applying the transformation to every element that isn’t missing.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func mapNonNil(_ transform: (WrappedElement) throws -> T?) rethrows -> Column
```

## Parameters 

`transform`  

A transformation closure.

## See Also

### Creating Transformed Columns

func map&lt;T>((Column&lt;WrappedElement>.Element) throws -> T?) rethrows -> Column&lt;T>

Creates a new column by applying a transformation to every element.

func filled(with: Self.WrappedElement) -> FilledColumn&lt;Self>

Generates a filled column by replacing missing elements with a value.

