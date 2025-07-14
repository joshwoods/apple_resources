

- UIKit
- UIAccessibility
-  hearingDevicePairedEar 

Type Property

# hearingDevicePairedEar

The current pairing status of Made for iPhone hearing devices.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
static var hearingDevicePairedEar: UIAccessibility.HearingDeviceEar { get }
```

## See Also

### Convenience functions

static func focusedElement(using: UIAccessibility.AssistiveTechnologyIdentifier?) -> Any?

Returns the accessibility element that’s currently in focus by the specified assistive app.

struct HearingDeviceEar

Constants that specify how a person is using a hearing device.

static func registerGestureConflictWithZoom()

Warns users that app-specific gestures conflict with the system-defined Zoom accessibility gestures.

static func requestGuidedAccessSession(enabled: Bool, completionHandler: (Bool) -> Void)

Transitions the app to or from Single App mode asynchronously.

static func zoomFocusChanged(zoomType: UIAccessibility.ZoomType, toFrame: CGRect, in: UIView)

Notifies the system when the app’s focus changes to a new location.

