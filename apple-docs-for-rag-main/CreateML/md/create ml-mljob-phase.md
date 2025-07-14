

- Create ML
- MLJob
-  phase 

Instance Property

# phase

Phase publisher.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
final var phase: AnyPublisher { get }
```

## See Also

### Receiving progress updates

var checkpoints: AnyPublisher&lt;MLCheckpoint, Never>

A publisher that sends a checkpoint for each of the session’s checkpoint intervals.

var result: AnyPublisher&lt;Result, any Error>

A publisher that provides a result when the training session has finished.

