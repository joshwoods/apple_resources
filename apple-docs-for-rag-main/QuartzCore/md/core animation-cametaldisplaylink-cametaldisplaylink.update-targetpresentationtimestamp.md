

- Core Animation
- CAMetalDisplayLink
- CAMetalDisplayLink.Update
-  targetPresentationTimestamp 

Instance Property

# targetPresentationTimestamp

The time the system estimates until the display of the next frame.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var targetPresentationTimestamp: CFTimeInterval { get }
```

## Discussion

Update your animations based on the time difference between this timestamp and the previous timestamp.

