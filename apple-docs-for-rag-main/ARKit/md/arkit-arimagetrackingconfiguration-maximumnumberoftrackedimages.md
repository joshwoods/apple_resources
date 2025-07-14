

- ARKit
- ARImageTrackingConfiguration
-  maximumNumberOfTrackedImages 

Instance Property

# maximumNumberOfTrackedImages

The number of image anchors to monitor closely for position and orientation updates.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var maximumNumberOfTrackedImages: Int { get set }
```

## Discussion

When you set a nonzero value for this property, the framework keeps that many image anchors up to date as the session progresses. The framework can track a maximum of four images simultaneously.

The word *track* in the property name refers to how the framework closely monitors the image’s physical position and orientation for any changes. If the image moves, the framework updates the associated ARImageAnchor transform with the new pose. ARKit checks for changes every frame.

ARKit tracks the first images it observes in the physical environment from the trackingImages set. When a session reaches the maximum number of tracked images, the framework attempts to track another member of the set only after one of the existing tracked images leaves the device’s view.

The default value is `1`.

## See Also

### Choosing Images to Track

var trackingImages: Set&lt;ARReferenceImage>

A set of images that ARKit searches for and tracks in the user’s environment.

