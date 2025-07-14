

- AVFoundation
-  AVAssetReaderOutputCaptionAdaptor 

Class

# AVAssetReaderOutputCaptionAdaptor

An object that reads caption group objects from an asset track that contains timed text.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVAssetReaderOutputCaptionAdaptor
```

## Topics

### Creating a Caption Adaptor

init(assetReaderTrackOutput: AVAssetReaderTrackOutput)

Creates a caption adaptor that reads from a track output.

### Accessing the Track Output

var assetReaderTrackOutput: AVAssetReaderTrackOutput

The associated asset reader track output.

### Managing the Validation Delegate

var validationDelegate: (any AVAssetReaderCaptionValidationHandling)?

A delegate object that handles callbacks to the caption adaptor.

protocol AVAssetReaderCaptionValidationHandling

A protocol that defines the methods for caption validation events.

### Reading Caption Groups

func nextCaptionGroup() -> AVCaptionGroup?

Returns the next caption group.

func captionsNotPresentInPreviousGroups(in: AVCaptionGroup) -> [AVCaption]

Returns the set of captions in the caption group that weren’t vended by the adaptor.

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

## See Also

### Reading and Writing

class AVAssetWriterInputCaptionAdaptor

An object that appends captions to an asset writer input.

