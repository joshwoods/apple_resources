

- ARKit
- ARWorldTrackingConfiguration
-  automaticImageScaleEstimationEnabled 

Instance Property

# automaticImageScaleEstimationEnabled

A flag that instructs the framework to estimate and set the scale of a detected or tracked image on your behalf.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
var automaticImageScaleEstimationEnabled: Bool { get set }
```

## Discussion

If set to true, ARKit uses its knowledge of the world to set an image anchor’s estimatedScaleFactor property, which corrects the image anchor’s position in the physical environment.

Enable this property when you want to detect different-sized versions of a reference image. ARKit must know the physical size of an image in the real world to accurately estimate its real-world position. Enable this property to tell ARKit to estimate a recognized image’s physical size before it calculates the real-world position.

## See Also

### Detecting or Tracking Images

var detectionImages: Set&lt;ARReferenceImage>!

A set of images that ARKit searches for in the user’s environment.

var maximumNumberOfTrackedImages: Int

The number of image anchors to monitor closely for position and orientation updates.

