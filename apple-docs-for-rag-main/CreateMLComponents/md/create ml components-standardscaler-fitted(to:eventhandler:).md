

- Create ML Components
- StandardScaler
-  fitted(to:eventHandler:) 

Instance Method

# fitted(to:eventHandler:)

Fits a transformer to a particular input sequence by computing the mean and standard deviation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func fitted(
    to input: S,
    eventHandler: EventHandler? = nil
) throws -> StandardScaler.Transformer where Element == S.Element, S : Sequence
```

