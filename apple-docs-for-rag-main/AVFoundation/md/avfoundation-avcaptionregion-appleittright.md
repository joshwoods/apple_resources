

- AVFoundation
- AVCaptionRegion
-  appleITTRight 

Type Property

# appleITTRight

The right region for iTT format captions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class var appleITTRight: AVCaptionRegion { get }
```

## Discussion

This region occupies the right 15% of the display area, and it uses a TBRL layout where a line progresses from top to bottom and the block extends from right to left. Lines are right justified.

## See Also

### Accessing Defined Regions

class var appleITTTop: AVCaptionRegion

The top region for iTT format captions.

class var appleITTBottom: AVCaptionRegion

The bottom region for iTT format captions.

class var appleITTLeft: AVCaptionRegion

The left region for iTT format captions.

class var subRipTextBottom: AVCaptionRegion

The bottom caption region for SubRip Text (SRT) format captions.

