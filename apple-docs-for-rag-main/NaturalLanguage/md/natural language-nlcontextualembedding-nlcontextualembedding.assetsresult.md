

- Natural Language
- NLContextualEmbedding
-  NLContextualEmbedding.AssetsResult 

Enumeration

# NLContextualEmbedding.AssetsResult

The status of an asset request.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
enum AssetsResult
```

## Topics

### Getting the result status

case available

A result that indicates assets are available.

case notAvailable

A result that indicates assets aren’t available.

case error

A result that indicates the framework encounters an error.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Requesting assets

func requestAssets(completionHandler: (NLContextualEmbedding.AssetsResult, (any Error)?) -> Void)

Requests assets for an embedding, if available.

