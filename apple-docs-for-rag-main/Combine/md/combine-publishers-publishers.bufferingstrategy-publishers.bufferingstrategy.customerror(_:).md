

- Combine
- Publishers
- Publishers.BufferingStrategy
-  Publishers.BufferingStrategy.customError(\_:) 

Case

# Publishers.BufferingStrategy.customError(\_:)

When the buffer is full, execute the closure to provide a custom error.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case customError(() -> Failure)
```

## See Also

### Buffering Strategies

case dropNewest

When the buffer is full, discard the newly received element.

case dropOldest

When the buffer is full, discard the oldest element in the buffer.

