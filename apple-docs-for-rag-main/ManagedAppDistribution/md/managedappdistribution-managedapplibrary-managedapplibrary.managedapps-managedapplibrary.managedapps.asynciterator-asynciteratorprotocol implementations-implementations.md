

- ManagedAppDistribution
- ManagedAppLibrary
- ManagedAppLibrary.ManagedApps
- ManagedAppLibrary.ManagedApps.AsyncIterator
-  AsyncIteratorProtocol Implementations 

API Collection

# AsyncIteratorProtocol Implementations

## Topics

### Instance Methods

func next() async throws(Self.Failure) -> Self.Element?

Default implementation of `next()` in terms of `next(isolation:)`, which is required to maintain backward compatibility with existing async iterators.

