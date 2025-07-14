

- AVFoundation
- AVAssetImageGenerator
-  AVAssetImageGenerator.Result 

Enumeration

# AVAssetImageGenerator.Result

Constants that indicate the result of an image generation request.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum Result
```

## Overview

The constants used in the block completion handler for generateCGImagesAsynchronously(forTimes:completionHandler:).

## Topics

### Results

case succeeded

A result that indicates that image generation succeeded.

case failed

A result that indicates that image generation failed.

case cancelled

A result that indicates you canceled image generation.

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

### Data Types

typealias AVAssetImageGeneratorCompletionHandler

A type alias for a closure that provides the result of an image generation request.

