

- TabularData
- FilledColumn
-  argmin() 

Instance Method

# argmin()

Returns the index of the element with the lowest value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

**iOS, iPadOS, macOS, tvOS, visionOS, watchOS**

``` source
func argmin() -> Base.Index?
```

**Mac Catalyst**

``` source
func argmin() -> FilledColumn.Index?
```

Available when `Base` conforms to `OptionalColumnProtocol` and `Base.WrappedElement` conforms to `Comparable`.

## See Also

### Finding an Element Index

func argmax() -> FilledColumn&lt;Base>.Index?

Returns the index of the element with the highest value.

