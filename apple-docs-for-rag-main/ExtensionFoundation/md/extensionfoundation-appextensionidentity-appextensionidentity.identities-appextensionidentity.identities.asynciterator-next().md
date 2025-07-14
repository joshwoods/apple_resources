

- ExtensionFoundation
- AppExtensionIdentity
- AppExtensionIdentity.Identities
- AppExtensionIdentity.Identities.AsyncIterator
-  next() 

Instance Method

# next()

Asynchronously advances to the next element and returns it.

macOS 13.0+

``` source
mutating func next() async -> [AppExtensionIdentity]?
```

## Return Value

The next element, if it exists, or `nil` to signal the end of the sequence.

## See Also

### Iterating the Sequence

struct AsyncIterator

The type of the asynchronous iterator created by this asynchronous sequence.

typealias Element

The type of element produced by this asynchronous sequence.

func makeAsyncIterator() -> AppExtensionIdentity.Identities.AsyncIterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

