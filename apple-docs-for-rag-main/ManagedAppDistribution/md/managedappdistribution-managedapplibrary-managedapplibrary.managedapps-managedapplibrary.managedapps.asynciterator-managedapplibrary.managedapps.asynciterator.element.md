

- ManagedAppDistribution
- ManagedAppLibrary
- ManagedAppLibrary.ManagedApps
- ManagedAppLibrary.ManagedApps.AsyncIterator
-  ManagedAppLibrary.ManagedApps.AsyncIterator.Element 

Type Alias

# ManagedAppLibrary.ManagedApps.AsyncIterator.Element

The type of element this asynchronous sequence produces.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
typealias Element = Result
```

## See Also

### Iterating

func next() async throws -> ManagedAppLibrary.ManagedApps.AsyncIterator.Element?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

