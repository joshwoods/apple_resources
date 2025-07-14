

- UIKit
- UIAccessibility
-  zoomFocusChanged(zoomType:toFrame:in:) 

Type Method

# zoomFocusChanged(zoomType:toFrame:in:)

Notifies the system when the app’s focus changes to a new location.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
static func zoomFocusChanged(
    zoomType type: UIAccessibility.ZoomType,
    toFrame frame: CGRect,
    in view: UIView
)
```

## Parameters 

`type`  

A `UIKit Functions` constant that identifies the type of Zoom.

`frame`  

The frame that’s currently zoomed, in screen coordinates.

`view`  

The view that contains the zoomed frame.

## See Also

### Convenience functions

static func focusedElement(using: UIAccessibility.AssistiveTechnologyIdentifier?) -> Any?

Returns the accessibility element that’s currently in focus by the specified assistive app.

static var hearingDevicePairedEar: UIAccessibility.HearingDeviceEar

The current pairing status of Made for iPhone hearing devices.

struct HearingDeviceEar

Constants that specify how a person is using a hearing device.

static func registerGestureConflictWithZoom()

Warns users that app-specific gestures conflict with the system-defined Zoom accessibility gestures.

static func requestGuidedAccessSession(enabled: Bool, completionHandler: (Bool) -> Void)

Transitions the app to or from Single App mode asynchronously.

