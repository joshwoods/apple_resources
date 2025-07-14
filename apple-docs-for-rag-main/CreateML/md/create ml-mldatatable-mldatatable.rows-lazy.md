

- Create ML
- MLDataTable
- MLDataTable.Rows
-  lazy 

Instance Property

# lazy

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var lazy: LazySequence { get }
```

## See Also

### Transforming a row collection

func compactMap&lt;ElementOfResult>((Self.Element) throws -> ElementOfResult?) rethrows -> [ElementOfResult]

Returns an array containing the non-`nil` results of calling the given transformation with each element of this sequence.

func reduce&lt;Result>(Result, (Result, Self.Element) throws -> Result) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

