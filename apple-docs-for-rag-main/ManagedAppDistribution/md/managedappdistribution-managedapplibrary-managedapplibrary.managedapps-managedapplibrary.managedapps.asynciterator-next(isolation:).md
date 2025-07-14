

- ManagedAppDistribution
- ManagedAppLibrary
- ManagedAppLibrary.ManagedApps
- ManagedAppLibrary.ManagedApps.AsyncIterator
-  next(isolation:) 

Instance Method

# next(isolation:)

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

iOS 18.0+iPadOS 18.0+visionOS 2.4+

``` source
func next(isolation actor: isolated (any Actor)?) async throws(ManagedAppLibrary.ManagedApps.AsyncIterator.Failure) -> ManagedAppLibrary.ManagedApps.AsyncIterator.Element?
```

