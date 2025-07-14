

- RealityKit
- Entity
- Entity.ChildCollection
- Entity.ChildCollection.IndexingIterator
-  forEach(\_:) 

Instance Method

# forEach(\_:)

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func forEach(_ body: (Self.Element) throws -> Void) rethrows
```

## Parameters 

`body`  

A closure that takes an element of the sequence as a parameter.

## Discussion

The two loops in the following example produce the same output:

```
let numberWords = ["one", "two", "three"]
for word in numberWords {
    print(word)
}
// Prints "one"
// Prints "two"
// Prints "three"

numberWords.forEach { word in
    print(word)
}
// Same as above
```

Using the `forEach` method is distinct from a `for`-`in` loop in two important ways:

1.  You cannot use a `break` or `continue` statement to exit the current call of the `body` closure or skip subsequent calls.

2.  Using the `return` statement in the `body` closure will exit only from the current call to `body`, not from any outer scope, and won’t skip subsequent calls.

## See Also

### Iterating over the collection

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

func next() -> Elements.Element?

Advances to the next element and returns it, or `nil` if no next element exists.

func makeIterator() -> Self

Returns an iterator over the elements of this sequence.

typealias Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

typealias Element

The type of element traversed by the iterator.

var underestimatedCount: Int

A value less than or equal to the number of elements in the sequence, calculated nondestructively.

