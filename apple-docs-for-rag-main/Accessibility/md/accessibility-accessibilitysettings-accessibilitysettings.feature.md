

- Accessibility
- AccessibilitySettings
-  AccessibilitySettings.Feature 

Enumeration

# AccessibilitySettings.Feature

Constants that describe specific Accessibility settings in the Settings app.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum Feature
```

## Topics

### Audio features

case personalVoiceAllowAppsToRequestToUse

A constant for opening the Settings app to the setting for Personal Voice \> Allow Apps to Request to Use.

### Accessibility feature structure creation

init?(rawValue: Int)

### Enumeration Cases

case allowAppsToAddAudioToCalls

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Opening the Settings app

static func openSettings(for: AccessibilitySettings.Feature) async throws

Opens the Settings app to a specific section of Accessibility settings.

