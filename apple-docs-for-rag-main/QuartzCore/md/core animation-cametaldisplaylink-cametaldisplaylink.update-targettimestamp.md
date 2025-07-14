

- Core Animation
- CAMetalDisplayLink
- CAMetalDisplayLink.Update
-  targetTimestamp 

Instance Property

# targetTimestamp

A deadline that indicates when your app needs to finish rendering to the drawable.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var targetTimestamp: CFTimeInterval { get }
```

## Discussion

Your app needs to call the drawable instance’s present() method before the deadline. GPU rendering can continue after this time, based on preferredFrameLatency. For more information on timing your app’s rendering, see metalDisplayLink(_:needsUpdate:).

## See Also

### Drawing the Next Frame

var drawable: any CAMetalDrawable

The Metal drawable your app uses to render the next frame.

var drawable: any CAMetalDrawable

The Metal drawable your app uses to render the next frame.

