

- TabularData
- FilledColumn
-  argmax() 

Instance Method

# argmax()

Returns the index of the element with the highest value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func argmax() -> FilledColumn.Index?
```

Available when `Base` conforms to `OptionalColumnProtocol` and `Base.WrappedElement` conforms to `Comparable`.

## See Also

### Finding an Element Index

func argmin() -> Base.Index?

Returns the index of the element with the lowest value.

