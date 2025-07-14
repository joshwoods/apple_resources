

- UIKit
- Accessibility for UIKit
-  Notification names 

API Collection

# Notification names

The names of notifications that the accessibility system generates.

## Topics

### UI changes

static let screenChanged: UIAccessibility.Notification

A notification that an app posts when a new view appears that occupies a major portion of the screen.

static let layoutChanged: UIAccessibility.Notification

A notification that an app posts when the layout of a screen changes.

static let pageScrolled: UIAccessibility.Notification

A notification that an app posts when a scroll action completes.

static let switchControlStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Switch Control setting changes.

static let elementFocusedNotification: NSNotification.Name

A notification that UIKit posts when an assistive app focuses on an accessibility element.

static let reduceTransparencyStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Reduce Transparency setting changes.

static let buttonShapesEnabledStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Button Shapes setting changes.

### VoiceOver

static let announcement: UIAccessibility.Notification

A notification that an app posts when it needs to convey an announcement to the assistive app.

static let voiceOverStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when VoiceOver starts or stops.

static let announcementDidFinishNotification: NSNotification.Name

A notification that UIKit posts when the system finishes reading an announcement.

let UIAccessibilityVoiceOverStatusChanged: String

A notification that UIKit posts when VoiceOver starts or stops.

Deprecated

### Text

static let boldTextStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Bold Text setting changes.

static let closedCaptioningStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the setting for Closed Captions + SDH changes.

### Colors

static let darkerSystemColorsStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Increase Contrast setting changes.

static let grayscaleStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Grayscale setting changes.

static let invertColorsStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the settings for inverted colors change.

### Assistive apps

static let assistiveTouchStatusDidChangeNotification: NSNotification.Name

A notification that indicates a change in the status of AssistiveTouch.

static let guidedAccessStatusDidChangeNotification: NSNotification.Name

A notification that indicates when a Guided Access session starts or ends.

static let pauseAssistiveTechnology: UIAccessibility.Notification

A notification that pauses an assistive app’s operations temporarily.

static let resumeAssistiveTechnology: UIAccessibility.Notification

A notification that resumes an assistive app’s operations temporarily.

struct AssistiveTechnologyIdentifier

Identifiers for assistive apps.

### Audio and speech

static let monoAudioStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when system audio changes from stereo to mono.

static let speakScreenStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Speak Screen setting changes.

static let speakSelectionStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Speak Selection setting changes.

static let hearingDevicePairedEarDidChangeNotification: NSNotification.Name

A notification that UIKit posts when there’s a change to the currently paired hearing devices.

### Motion

static let reduceMotionStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Reduce Motion setting changes.

static let shakeToUndoDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Shake to Undo setting changes.

## See Also

### Notifications

Notification dictionary keys

Handle notifications with keys in the user info dictionary.

static func post(notification: UIAccessibility.Notification, argument: Any?)

Posts a notification to assistive apps.

