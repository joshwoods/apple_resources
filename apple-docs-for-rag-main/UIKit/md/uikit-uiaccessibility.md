

- UIKit
-  UIAccessibility 

Structure

# UIAccessibility

A namespace for accessibility symbols for UIKit apps.

iOSiPadOSMac CatalysttvOSvisionOSwatchOS

``` source
struct UIAccessibility
```

## Topics

### System notifications

static let announcementDidFinishNotification: NSNotification.Name

A notification that UIKit posts when the system finishes reading an announcement.

static let elementFocusedNotification: NSNotification.Name

A notification that UIKit posts when an assistive app focuses on an accessibility element.

### App notifications

static func post(notification: UIAccessibility.Notification, argument: Any?)

Posts a notification to assistive apps.

struct Notification

An accessibility notification that an app can send.

### Notification keys

static let announcementStringValueUserInfoKey: String

The text of the announcement.

static let announcementWasSuccessfulUserInfoKey: String

A Boolean value that indicates whether the announcement is successful.

static let focusedElementUserInfoKey: String

The element currently in focus by the assistive app.

static let unfocusedElementUserInfoKey: String

The element previously in focus by the assistive app.

static let assistiveTechnologyUserInfoKey: String

The identifier of the assistive app.

### VoiceOver

static var isVoiceOverRunning: Bool

A Boolean value that indicates whether VoiceOver is in an enabled state.

static let voiceOverStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when VoiceOver starts or stops.

### Switch Control

static var isSwitchControlRunning: Bool

A Boolean value that indicates whether the Switch Control setting is in an enabled state.

static let switchControlStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Switch Control setting changes.

### AssistiveTouch

static var isAssistiveTouchRunning: Bool

A Boolean value that indicates whether AssistiveTouch is in an enabled state.

static let assistiveTouchStatusDidChangeNotification: NSNotification.Name

A notification that indicates a change in the status of AssistiveTouch.

### Autoplay videos

static var isVideoAutoplayEnabled: Bool

A Boolean value that indicates whether the Auto-Play Video Previews setting is in an enabled state.

static let videoAutoplayStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Auto-Play Video Previews setting changes.

### Bold text

static var isBoldTextEnabled: Bool

A Boolean value that indicates whether the Bold Text setting is in an enabled state.

static let boldTextStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Bold Text setting changes.

### Button shapes

static var buttonShapesEnabled: Bool

A Boolean value that indicates whether the Button Shapes setting is in an enabled state.

static let buttonShapesEnabledStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Button Shapes setting changes.

### Closed captions

static var isClosedCaptioningEnabled: Bool

A Boolean value that indicates whether the Closed Captions + SDH setting is in an enabled state.

static let closedCaptioningStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the setting for Closed Captions + SDH changes.

### Cross-fade transitions

static var prefersCrossFadeTransitions: Bool

A Boolean value that indicates whether the Reduce Motion and the Prefer Cross-Fade Transitions settings are in an enabled state.

static let prefersCrossFadeTransitionsStatusDidChange: NSNotification.Name

A notification that UIKit posts when the system’s Prefer Cross-Fade Transitions setting changes.

### Differentiate without color

static var shouldDifferentiateWithoutColor: Bool

A Boolean value that indicates whether the Differentiate Without Color setting is in an enabled state.

static let differentiateWithoutColorDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Differentiate Without Color setting changes.

### Grayscale

static var isGrayscaleEnabled: Bool

A Boolean value that indicates whether the Color Filters and the Grayscale settings are in an enabled state.

static let grayscaleStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Grayscale setting changes.

### Guided Access

static var isGuidedAccessEnabled: Bool

A Boolean value that indicates whether the Guided Access setting is in an enabled state.

static let guidedAccessStatusDidChangeNotification: NSNotification.Name

A notification that indicates when a Guided Access session starts or ends.

static func requestGuidedAccessSession(enabled: Bool, completionHandler: (Bool) -> Void)

Transitions the app to or from Single App mode asynchronously.

static func configureForGuidedAccess(features: UIGuidedAccessAccessibilityFeature, enabled: Bool, completionHandler: (Bool, (any Error)?) -> Void)

Enables or disables the specified accessibility features while using Guided Access.

static func guidedAccessRestrictionState(forIdentifier: String) -> UIAccessibility.GuidedAccessRestrictionState

Returns the restriction state for the specified guided access restriction.

enum GuidedAccessRestrictionState

Constants that describe the state of a restriction, either allow or deny.

static let guidedAccessErrorDomain: String

A string that identifies the Guided Access error domain.

struct GuidedAccessError

A Guided Access error.

### Hearing devices

static var hearingDevicePairedEar: UIAccessibility.HearingDeviceEar

The current pairing status of Made for iPhone hearing devices.

static let hearingDevicePairedEarDidChangeNotification: NSNotification.Name

A notification that UIKit posts when there’s a change to the currently paired hearing devices.

### Increase contrast

static var isDarkerSystemColorsEnabled: Bool

A Boolean value that indicates whether the Increase Contrast setting is in an enabled state.

static let darkerSystemColorsStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Increase Contrast setting changes.

### Invert colors

static var isInvertColorsEnabled: Bool

A Boolean value that indicates whether the Classic Invert setting is in an enabled state.

static let invertColorsStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the settings for inverted colors change.

### Mono audio

static var isMonoAudioEnabled: Bool

A Boolean value that indicates whether the Mono Audio setting is in an enabled state.

static let monoAudioStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when system audio changes from stereo to mono.

### On and off labels

static var isOnOffSwitchLabelsEnabled: Bool

A Boolean value that indicates whether the On/Off Labels setting is in an enabled state.

static let onOffSwitchLabelsDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s On/Off Labels setting changes.

### Reduce motion

static var isReduceMotionEnabled: Bool

A Boolean value that indicates whether the Reduce Motion setting is in an enabled state.

static let reduceMotionStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Reduce Motion setting changes.

### Reduce transparency

static var isReduceTransparencyEnabled: Bool

A Boolean value that indicates whether the Reduce Transparency setting is in an enabled state.

static let reduceTransparencyStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Reduce Transparency setting changes.

### Shake to undo

static var isShakeToUndoEnabled: Bool

A Boolean value that indicates whether the Shake to Undo setting is in an enabled state.

static let shakeToUndoDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Shake to Undo setting changes.

### Spoken content

static var isSpeakScreenEnabled: Bool

A Boolean value that indicates whether the Speak Screen setting is in an enabled state.

static let speakScreenStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Speak Screen setting changes.

static var isSpeakSelectionEnabled: Bool

A Boolean value that indicates whether the Speak Selection setting is in an enabled state.

static let speakSelectionStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Speak Selection setting changes.

### Conversions

static func convertToScreenCoordinates(UIBezierPath, in: UIView) -> UIBezierPath

Converts the specified path object to screen coordinates and returns a new path object with the results.

static func convertToScreenCoordinates(CGRect, in: UIView) -> CGRect

Converts the specified rectangle from view coordinates to screen coordinates.

### Convenience functions

static func focusedElement(using: UIAccessibility.AssistiveTechnologyIdentifier?) -> Any?

Returns the accessibility element that’s currently in focus by the specified assistive app.

static func registerGestureConflictWithZoom()

Warns users that app-specific gestures conflict with the system-defined Zoom accessibility gestures.

static func zoomFocusChanged(zoomType: UIAccessibility.ZoomType, toFrame: CGRect, in: UIView)

Notifies the system when the app’s focus changes to a new location.

### Constants

struct UIAccessibilityTraits

Constants that describe how an accessibility element behaves.

struct AssistiveTechnologyIdentifier

Identifiers for assistive apps.

struct HearingDeviceEar

Constants that specify how a person is using a hearing device.

enum UIAccessibilityContainerType

Constants that indicate the type of content in a data-based container.

enum UIAccessibilityNavigationStyle

Constants that describe how to navigate an object’s elements with an assistive app.

enum UIAccessibilityScrollDirection

The direction of a scrolling action.

enum ZoomType

The types of system Zoom that can be in effect.

struct DirectTouchOptions

Constants that configure how VoiceOver produces audio for direct touch areas.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Supporting types

typealias AXArrayReturnBlock

typealias AXAttributedStringArrayReturnBlock

typealias AXAttributedStringReturnBlock

typealias AXBoolReturnBlock

typealias AXContainerTypeReturnBlock

typealias AXCustomActionsReturnBlock

typealias AXCustomRotorsReturnBlock

typealias AXNavigationStyleReturnBlock

typealias AXObjectReturnBlock

typealias AXPathReturnBlock

typealias AXPointReturnBlock

typealias AXRectReturnBlock

typealias AXStringArrayReturnBlock

typealias AXStringReturnBlock

typealias AXTextualContextReturnBlock

