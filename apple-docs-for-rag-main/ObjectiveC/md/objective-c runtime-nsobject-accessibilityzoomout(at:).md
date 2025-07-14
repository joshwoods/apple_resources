

- Objective-C Runtime
- NSObject
-  accessibilityZoomOut(at:) 

Instance Method

# accessibilityZoomOut(at:)

Zooms out from the content at the specified point.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
func accessibilityZoomOut(at point: CGPoint) -> Bool
```

## Parameters 

`point`  

The point where a person performs the zoom out action.

## Return Value

YES if this method successfully handles zooming; otherwise, NO. By default, this method returns NO.

## Discussion

If your element has the supportsZoom trait, you need to implement this method and accessibilityZoomIn(at:). Use this method to zoom out from the specified point. For example, if the element allows a pinch gesture to zoom out from the view’s content, implement this method so that the VoiceOver zoom action receives the same behavior.

