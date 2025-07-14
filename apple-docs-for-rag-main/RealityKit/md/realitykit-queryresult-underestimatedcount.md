

- RealityKit
- QueryResult
-  underestimatedCount 

Instance Property

# underestimatedCount

A value less than or equal to the number of elements in the sequence, calculated nondestructively.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
var underestimatedCount: Int { get }
```

## Discussion

The default implementation returns 0. If you provide your own implementation, make sure to compute the value nondestructively.

Complexity

O(1), except if the sequence also conforms to `Collection`. In this case, see the documentation of `Collection.underestimatedCount`.

## See Also

### Iterating over a sequence’s elements

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

