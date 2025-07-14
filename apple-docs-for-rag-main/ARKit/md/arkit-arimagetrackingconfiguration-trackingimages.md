

- ARKit
- ARImageTrackingConfiguration
-  trackingImages 

Instance Property

# trackingImages

A set of images that ARKit searches for and tracks in the user’s environment.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var trackingImages: Set { get set }
```

## Discussion

Add members to this set for each image that ARKit searches for in the user’s environment. When ARKit observes a matching image, the framework creates an ARImageAnchor object and adds it to the session. If you set maximumNumberOfTrackedImages to a value greater than `1`, ARKit tracks multiple images as the session progresses, up to a maximum of four.

To define the reference images that this property contains, create an asset catalog in Xcode or create ARReferenceImage objects programmatically. For an example, see Tracking and altering images.

## See Also

### Choosing Images to Track

var maximumNumberOfTrackedImages: Int

The number of image anchors to monitor closely for position and orientation updates.

