

- Create ML
- MLDataTable
- MLDataTable.Rows
-  makeIterator() 

Instance Method

# makeIterator()

Returns an iterator over the elements of the collection.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func makeIterator() -> IndexingIterator
```

Available when `Iterator` is `IndexingIterator`.

## See Also

### Iterating over a row collection’s rows

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

