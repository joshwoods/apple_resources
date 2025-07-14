

- AVFoundation
- AVAssetVariant
- AVAssetVariant.VideoAttributes
- AVAssetVariant.VideoAttributes.LayoutAttributes
-  stereoViewComponents 

Instance Property

# stereoViewComponents

Attributes that describe the video’s stereo components.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var stereoViewComponents: CMStereoViewComponents { get }
```

## Discussion

In the case of 3D or stereoscopic content, the value contains leftEye and rightEye components. In the case of monoscopic content, this value is kCMStereoView_None.

