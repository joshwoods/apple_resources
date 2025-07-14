

- Swift
- Set
-  init(\_:) 

Initializer

# init(\_:)

Creates a new set from a finite sequence of items.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(_ sequence: Source) where Element == Source.Element, Source : Sequence
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`sequence`  

The elements to use as members of the new set.

## Discussion

Use this initializer to create a new set from an existing sequence, for example, an array or a range.

```
let validIndices = Set(0..

This initializer can also be used to restore set methods after performing sequence operations such as `filter(_:)` or `map(_:)` on a set. For example, after filtering a set of prime numbers to remove any below 10, you can create a new set by using this initializer.

```
let primes: Set = [2, 3, 5, 7, 11, 13, 17, 19, 23]
let laterPrimes = Set(primes.lazy.filter { $0 > 10 })
print(laterPrimes)
// Prints "[17, 19, 23, 11, 13]"
```

## See Also

### Creating a Set

init()

Creates an empty set.

init(minimumCapacity: Int)

Creates an empty set with preallocated space for at least the specified number of elements.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

