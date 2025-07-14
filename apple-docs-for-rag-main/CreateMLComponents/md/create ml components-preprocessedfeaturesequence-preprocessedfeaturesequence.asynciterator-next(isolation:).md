

- Create ML Components
- PreprocessedFeatureSequence
- PreprocessedFeatureSequence.AsyncIterator
-  next(isolation:) 

Instance Method

# next(isolation:)

Default implementation of `next(isolation:)` in terms of `next()`, which is required to maintain backward compatibility with existing async iterators.

Create ML ComponentsSwiftiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func next(isolation actor: isolated (any Actor)?) async throws(Self.Failure) -> Self.Element?
```

