

- TabularData
- Column
-  append(contentsOf:) 

Instance Method

# append(contentsOf:)

Appends a sequence of optional values to the column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func append(contentsOf sequence: S) where S : Sequence, S.Element == WrappedElement?
```

## Parameters 

`sequence`  

A sequence of optional elements.

## See Also

### Adding Elements

func append(WrappedElement)

Appends a nonoptional value to the column.

func append(Column&lt;WrappedElement>.Element)

Appends an optional value to the column.

func append&lt;S>(contentsOf: S)

Appends a sequence of nonoptional values to the column.

