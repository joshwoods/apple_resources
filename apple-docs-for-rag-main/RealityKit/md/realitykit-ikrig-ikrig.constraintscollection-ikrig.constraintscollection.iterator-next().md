

- RealityKit
- IKRig
- IKRig.ConstraintsCollection
- IKRig.ConstraintsCollection.Iterator
-  next() 

Instance Method

# next()

Advances to the next element and returns it, or `nil` if no next element exists.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
mutating func next() -> IKRig.ConstraintsCollection.Element?
```

## Return Value

The next element in the underlying sequence, if a next element exists; otherwise, `nil`.

## Discussion

Repeatedly calling this method returns, in order, all the elements of the underlying sequence. As soon as the sequence has run out of elements, all subsequent calls return `nil`.

You must not call this method if any other copy of this iterator has been advanced with a call to its `next()` method.

The following example shows how an iterator can be used explicitly to emulate a `for`-`in` loop. First, retrieve a sequence’s iterator, and then call the iterator’s `next()` method until it returns `nil`.

```
let numbers = [2, 3, 5, 7]
var numbersIterator = numbers.makeIterator()

while let num = numbersIterator.next() {
    print(num)
}
// Prints "2"
// Prints "3"
// Prints "5"
// Prints "7"
```

