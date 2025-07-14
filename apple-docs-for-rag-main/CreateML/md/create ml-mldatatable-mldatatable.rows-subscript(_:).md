

- Create ML
- MLDataTable
- MLDataTable.Rows
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Subscript by index. This returns a row in the data table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(index: Int) -> MLDataTable.Rows.Element { get }
```

## See Also

### Accessing rows

var first: Self.Element?

The first element of the collection.

var last: Self.Element?

The last element of the collection.

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

