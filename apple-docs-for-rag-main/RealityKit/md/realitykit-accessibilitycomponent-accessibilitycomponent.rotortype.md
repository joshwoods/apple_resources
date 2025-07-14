

- RealityKit
- AccessibilityComponent
-  AccessibilityComponent.RotorType 

Enumeration

# AccessibilityComponent.RotorType

A context-sensitive event that helps VoiceOver users find the next instance of a related element.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS

``` source
enum RotorType
```

## Topics

### Operators

static func == (AccessibilityComponent.RotorType, AccessibilityComponent.RotorType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case custom(LocalizedStringResource)

case system(UIAccessibilityCustomRotor.SystemRotorType)

A rotor type provided by the system.

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

struct CustomContent

A CustomContent struct contains the accessibility strings for the labels you apply to your accessibility content.

enum AccessibilityEvents

