

- ActivityKit
- Activity
- Activity.ActivityStateUpdates
- Activity.ActivityStateUpdates.Iterator
-  AsyncIteratorProtocol Implementations 

API Collection

# AsyncIteratorProtocol Implementations

## Topics

### Instance Methods

func next(isolation: isolated (any Actor)?) async throws(Self.Failure) -> Self.Element?

Default implementation of `next(isolation:)` in terms of `next()`, which is required to maintain backward compatibility with existing async iterators.

