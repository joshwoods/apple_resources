

- UIKit
- UIAccessibility
-  focusedElement(using:) 

Type Method

# focusedElement(using:)

Returns the accessibility element that’s currently in focus by the specified assistive app.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
static func focusedElement(using assistiveTechnologyIdentifier: UIAccessibility.AssistiveTechnologyIdentifier?) -> Any?
```

## Return Value

The element that is currently focused by the specified assistive technology or the element that was most recently focused, if no technology is specified.

## See Also

### Convenience functions

static var hearingDevicePairedEar: UIAccessibility.HearingDeviceEar

The current pairing status of Made for iPhone hearing devices.

struct HearingDeviceEar

Constants that specify how a person is using a hearing device.

static func registerGestureConflictWithZoom()

Warns users that app-specific gestures conflict with the system-defined Zoom accessibility gestures.

static func requestGuidedAccessSession(enabled: Bool, completionHandler: (Bool) -> Void)

Transitions the app to or from Single App mode asynchronously.

static func zoomFocusChanged(zoomType: UIAccessibility.ZoomType, toFrame: CGRect, in: UIView)

Notifies the system when the app’s focus changes to a new location.

