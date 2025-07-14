

- AVFoundation
-  AVAssetWriterInputPassDescription 

Class

# AVAssetWriterInputPassDescription

An object that defines the interface to query for the requirements of the current pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetWriterInputPassDescription
```

## Topics

### Getting Source Time Ranges

var sourceTimeRanges: [NSValue]

An array of time ranges.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Performing Multiple-Pass Encoding

var canPerformMultiplePasses: Bool

A Boolean value that indicates whether the input may perform multiple passes over appended media data.

var currentPassDescription: AVAssetWriterInputPassDescription?

An object that describes the requirements for the current pass.

func markCurrentPassAsFinished()

Tells the input to analyze the appended media to determine whether it can improve the results by reencoding certain segments.

var performsMultiPassEncodingIfSupported: Bool

A Boolean value that indicates whether the input attempts to encode the source media data using multiple passes.

func respondToEachPassDescription(on: dispatch_queue_t, using: () -> Void)

Tells the input to invoke a callback whenever it begins a new pass.

