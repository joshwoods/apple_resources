

- TabularData
- Column
-  transform(\_:) 

Instance Method

# transform(\_:)

Applies a transformation to every element that isn’t missing.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func transform(_ transform: (WrappedElement) throws -> WrappedElement) rethrows
```

## Parameters 

`transform`  

A transformation closure.

## See Also

### Transforming a Column

func transform((Column&lt;WrappedElement>.Element) throws -> Column&lt;WrappedElement>.Element) rethrows

Applies a transformation to every element in the column.

