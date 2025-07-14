

- AVFoundation
- AVCaptionRegion
-  appleITTTop 

Type Property

# appleITTTop

The top region for iTT format captions.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class var appleITTTop: AVCaptionRegion { get }
```

## Discussion

This region is available when working with iTT captions. It occupies the top 15% of the display area, and it uses a LRTB layout where a line progresses from left to right and the block extends from top to bottom. Lines are top justified.

## See Also

### Accessing Defined Regions

class var appleITTBottom: AVCaptionRegion

The bottom region for iTT format captions.

class var appleITTLeft: AVCaptionRegion

The left region for iTT format captions.

class var appleITTRight: AVCaptionRegion

The right region for iTT format captions.

class var subRipTextBottom: AVCaptionRegion

The bottom caption region for SubRip Text (SRT) format captions.

