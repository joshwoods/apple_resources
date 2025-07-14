

- AVFoundation
- AVCaptionRegion
-  appleITTLeft 

Type Property

# appleITTLeft

The left region for iTT format captions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class var appleITTLeft: AVCaptionRegion { get }
```

## Discussion

This region occupies the left 15% of the display area, and it uses a TBRL layout where a line progresses from top to bottom and the block extends from right to left. Lines are left justified.

## See Also

### Accessing Defined Regions

class var appleITTTop: AVCaptionRegion

The top region for iTT format captions.

class var appleITTBottom: AVCaptionRegion

The bottom region for iTT format captions.

class var appleITTRight: AVCaptionRegion

The right region for iTT format captions.

class var subRipTextBottom: AVCaptionRegion

The bottom caption region for SubRip Text (SRT) format captions.

