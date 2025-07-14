

- AVFoundation
- AVCapturePhotoOutput
-  isConstantColorSupported 

Instance Property

# isConstantColorSupported

A Boolean value that indicates whether a photo output supports constant color capture.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var isConstantColorSupported: Bool { get }
```

## Discussion

The light sources illuminating a scene affect an object’s color in a photograph, so the color of the same object captured in warm light might look significantly different than in colder light. In some cases, ambient light-induced color variation is undesirable, and you may prefer an estimate of what these materials would look like under a standard light such as daylight (D65), regardless of the lighting conditions at the time of capture. Some devices are capable of producing such constant color photos.

Constant color captures require the flash to fire and may require a pre-flash sequence to determine the correct focus and exposure, therefore it might take several seconds to acquire a constant color photo. Due to this flash requirement, you can only take a constant color capture with AVCaptureDevice.FlashMode.auto or AVCaptureDevice.FlashMode.on as the flash mode, otherwise the system throws an exception.

You can only achieve constant color when the flash has a discernible effect on the scene, so it may not perform well in bright conditions such as direct sunlight. Use the photo’s constantColorConfidenceMap property to examine the confidence level, and therefore the usefulness, of each region of a constant color photo.

The property value is true if the session’s current configuration allows the output to capture photos with constant color.

When switching cameras or formats this property may change. When this property changes from true to false, the value of isConstantColorEnabled also reverts to false. If you’ve previously opted in to constant color and then change configurations, you may need to set the value of isConstantColorEnabled to true again.

This property is key-value observable.

## See Also

### Configuring Constant Color

var isConstantColorEnabled: Bool

A Boolean value that indicates whether the photo output configures the render pipeline to perform constant color capture.

