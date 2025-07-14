

- ExtensionFoundation
- AppExtensionIdentity
- AppExtensionIdentity.Identities
-  AppExtensionIdentity.Identities.Element 

Type Alias

# AppExtensionIdentity.Identities.Element

The type of element produced by this asynchronous sequence.

macOS 13.0+

``` source
typealias Element = [AppExtensionIdentity]
```

## See Also

### Iterating the Sequence

func next() async -> [AppExtensionIdentity]?

Asynchronously advances to the next element and returns it.

struct AsyncIterator

The type of the asynchronous iterator created by this asynchronous sequence.

func makeAsyncIterator() -> AppExtensionIdentity.Identities.AsyncIterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

