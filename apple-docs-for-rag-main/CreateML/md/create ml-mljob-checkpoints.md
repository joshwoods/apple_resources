

- Create ML
- MLJob
-  checkpoints 

Instance Property

# checkpoints

A publisher that sends a checkpoint for each of the session’s checkpoint intervals.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
final var checkpoints: AnyPublisher { get }
```

## See Also

### Receiving progress updates

var result: AnyPublisher&lt;Result, any Error>

A publisher that provides a result when the training session has finished.

var phase: AnyPublisher&lt;MLPhase, Never>

Phase publisher.

