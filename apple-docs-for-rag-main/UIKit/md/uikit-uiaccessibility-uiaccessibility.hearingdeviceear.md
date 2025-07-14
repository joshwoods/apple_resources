

- UIKit
- UIAccessibility
-  UIAccessibility.HearingDeviceEar 

Structure

# UIAccessibility.HearingDeviceEar

Constants that specify how a person is using a hearing device.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct HearingDeviceEar
```

## Topics

### Constants

static var left: UIAccessibility.HearingDeviceEar

A constant that represents the left ear.

static var right: UIAccessibility.HearingDeviceEar

A constant that represents the right ear.

static var both: UIAccessibility.HearingDeviceEar

A constant that represents both ears.

### Initializers

init(rawValue: UInt)

Creates a structure that represents a hearing-device ear with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Convenience functions

static func focusedElement(using: UIAccessibility.AssistiveTechnologyIdentifier?) -> Any?

Returns the accessibility element that’s currently in focus by the specified assistive app.

static var hearingDevicePairedEar: UIAccessibility.HearingDeviceEar

The current pairing status of Made for iPhone hearing devices.

static func registerGestureConflictWithZoom()

Warns users that app-specific gestures conflict with the system-defined Zoom accessibility gestures.

static func requestGuidedAccessSession(enabled: Bool, completionHandler: (Bool) -> Void)

Transitions the app to or from Single App mode asynchronously.

static func zoomFocusChanged(zoomType: UIAccessibility.ZoomType, toFrame: CGRect, in: UIView)

Notifies the system when the app’s focus changes to a new location.

