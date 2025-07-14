

- ShazamKit
- SHMatchedMediaItem
-  confidence 

Instance Property

# confidence

The level of confidence in the match result.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
var confidence: Float { get }
```

## Discussion

Note

This may be fetched using the key @c SHMediaItemConfidence

The value ranges from 0.0 to 1.0, where 1.0 indicates the highest level of confidence.

