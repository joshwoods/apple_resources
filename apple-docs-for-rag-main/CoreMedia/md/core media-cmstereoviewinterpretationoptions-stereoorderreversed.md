

- Core Media
- CMStereoViewInterpretationOptions
-  stereoOrderReversed 

Type Property

# stereoOrderReversed

Changes the default ordering of eye data, switching it from left-to-right to right-to-left.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var stereoOrderReversed: CMStereoViewInterpretationOptions { get }
```

## Discussion

Setting the stereoOrderReversed flag changes interpretations of geometry and affects internal storage.

## See Also

### Stereo View Options

static var additionalViews: CMStereoViewInterpretationOptions

A flag indicating that the video content contains additional views beyond the left or right eye.

