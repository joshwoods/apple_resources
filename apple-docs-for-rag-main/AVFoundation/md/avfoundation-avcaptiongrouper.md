

- AVFoundation
-  AVCaptionGrouper 

Class

# AVCaptionGrouper

An object that analyzes the temporal overlaps of caption objects to create caption groups for each span of concurrent captions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVCaptionGrouper
```

## Topics

### Adding Captions

func add(AVCaption)

Adds a caption to the pending group.

### Generating Captions Groups

func flushAddedCaptions(upTo: CMTime) -> [AVCaptionGroup]

Creates caption groups for the captions you enqueue up to the time.

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

### Groups

class AVCaptionGroup

An object that represents zero or more captions that intersect in time.

