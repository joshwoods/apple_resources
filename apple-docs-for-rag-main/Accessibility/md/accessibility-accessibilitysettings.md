

- Accessibility
-  AccessibilitySettings 

Structure

# AccessibilitySettings

A structure for working with accessibility system settings.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct AccessibilitySettings
```

## Topics

### Opening the Settings app

static func openSettings(for: AccessibilitySettings.Feature) async throws

Opens the Settings app to a specific section of Accessibility settings.

enum Feature

Constants that describe specific Accessibility settings in the Settings app.

### Pausing animated images

Animated images

Pause animations in animated images in your app when people turn off the Animated Images setting.

static var animatedImagesEnabled: Bool

A Boolean value that indicates whether the system setting for playing animated images is on.

static var animatedImagesEnabledDidChangeNotification: Notification.Name

A notification that posts when the system setting for playing animated images changes.

### Customizing vertical text layout

Horizontal text

Lay out vertical text horizontally in your app when people turn on the Prefer Horizontal Text setting.

static var prefersHorizontalTextLayout: Bool

A Boolean value that indicates whether the system setting to prefer horizontal text for languages that support both vertical and horizontal text layout is on.

static var prefersHorizontalTextLayoutDidChangeNotification: Notification.Name

A notification that posts when the system setting to prefer horizontal text for languages that support both vertical and horizontal text layout changes.

### Supporting head-anchored content

static var prefersHeadAnchorAlternative: Bool

A Boolean value that indicates the person’s preference for content that follows their head position.

static var prefersHeadAnchorAlternativeDidChangeNotification: Notification.Name

A notification that posts when the system setting for head-anchored content changes.

### Reducing animation for text insertion indicators

static var prefersNonBlinkingTextInsertionIndicator: Bool

A Boolean value that indicates whether the system setting to prefer a nonblinking cursor in editable text fields is on.

static let prefersNonBlinkingTextInsertionIndicatorDidChangeNotification: NSNotification.Name

A notification that posts when the system setting to prefer a nonblinking cursor in editable text fields changes.

### Checking if Assistive Access is running

static var isAssistiveAccessEnabled: Bool

A Boolean value that indicates whether Assistive Access is running.

### Creating an accessibility settings structure

init()

## Relationships

### Conforms To

- BitwiseCopyable

