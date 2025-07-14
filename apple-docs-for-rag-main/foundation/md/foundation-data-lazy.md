

- Foundation
- Data
-  lazy 

Instance Property

# lazy

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

FoundationSwiftiOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var lazy: LazySequence { get }
```

## See Also

### Transforming Data

func reduce&lt;Result>(Result, (Result, Self.Element) throws -> Result) rethrows -> Result

Returns the result of combining the elements of the sequence using the given closure.

