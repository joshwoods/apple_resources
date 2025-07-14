

- AVFoundation
-  AVAssetWriterInputCaptionAdaptor 

Class

# AVAssetWriterInputCaptionAdaptor

An object that appends captions to an asset writer input.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVAssetWriterInputCaptionAdaptor
```

## Topics

### Creating a Caption Adaptor

init(assetWriterInput: AVAssetWriterInput)

Creates a new caption adaptor that writes to the specified asset writer input.

### Accessing the Writer Input

var assetWriterInput: AVAssetWriterInput

The associated asset writer input.

### Appending Captions

func append(AVCaption) -> Bool

Appends a caption to the writer input.

func append(AVCaptionGroup) -> Bool

Appends a caption group that the system writes to the output.

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

class AVAssetReaderOutputCaptionAdaptor

An object that reads caption group objects from an asset track that contains timed text.

