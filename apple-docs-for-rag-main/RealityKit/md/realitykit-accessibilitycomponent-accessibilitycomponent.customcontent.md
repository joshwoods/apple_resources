

- RealityKit
- AccessibilityComponent
-  AccessibilityComponent.CustomContent 

Structure

# AccessibilityComponent.CustomContent

A CustomContent struct contains the accessibility strings for the labels you apply to your accessibility content.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS

``` source
struct CustomContent
```

## Topics

### Operators

static func == (AccessibilityComponent.CustomContent, AccessibilityComponent.CustomContent) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(label: LocalizedStringResource, value: LocalizedStringResource, importance: AXCustomContent.Importance)

Creates a new CustomContent with the given label, value, and importance.

### Instance Properties

var importance: AXCustomContent.Importance

Determines when to output custom accessibility content.

var label: LocalizedStringResource

A localized string key that identifies the label for this content.

var value: LocalizedStringResource

A localized string key that provides a value for the label.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Accessibility

Improving the Accessibility of RealityKit Apps

Incorporate assistive technologies in your augmented reality app.

struct AccessibilityComponent

A component that stores accessibility information for an entity.

struct SupportedActions

A custom action that can be invoked on an entity in response to specific user cues.

enum RotorType

A context-sensitive event that helps VoiceOver users find the next instance of a related element.

enum AccessibilityEvents

