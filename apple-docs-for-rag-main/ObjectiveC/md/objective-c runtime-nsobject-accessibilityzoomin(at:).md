

- Objective-C Runtime
- NSObject
-  accessibilityZoomIn(at:) 

Instance Method

# accessibilityZoomIn(at:)

Zooms in on the content at the specified point.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
func accessibilityZoomIn(at point: CGPoint) -> Bool
```

## Parameters 

`point`  

The point where a person performs the zoom in action.

## Return Value

YES if this method successfully handles zooming; otherwise, NO. By default, this method returns NO.

## Discussion

If your element has the supportsZoom trait, you need to implement this method and accessibilityZoomOut(at:). Use this method to zoom in at the specified point. For example, if the element allows an expand gesture to zoom in to the view’s content, implement this method so that the VoiceOver zoom action receives the same behavior.

