

- AVFoundation
- AVCaptionRegion
-  subRipTextBottom 

Type Property

# subRipTextBottom

The bottom caption region for SubRip Text (SRT) format captions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class var subRipTextBottom: AVCaptionRegion { get }
```

## Discussion

This region is suitable for SRT format, and it occupies the entire video display area. The region uses a AVCaptionRegion.WritingMode.leftToRightAndTopToBottom writing mode, where a line progresses left to right and the block extends from top to bottom. The system stacks each line of text with bottom justification.

## See Also

### Accessing Defined Regions

class var appleITTTop: AVCaptionRegion

The top region for iTT format captions.

class var appleITTBottom: AVCaptionRegion

The bottom region for iTT format captions.

class var appleITTLeft: AVCaptionRegion

The left region for iTT format captions.

class var appleITTRight: AVCaptionRegion

The right region for iTT format captions.

