

- SwiftUI
-  AccessibilityTechnologies 

Structure

# AccessibilityTechnologies

Accessibility technologies available to the system.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AccessibilityTechnologies
```

## Topics

### Getting technology types

static let switchControl: AccessibilityTechnologies

The value that represents a Switch Control, allowing the use of the entire system using controller buttons, a breath-controlled switch or similar hardware.

static let voiceOver: AccessibilityTechnologies

The value that represents the VoiceOver screen reader, allowing use of the system without seeing the screen visually.

### Creating a technology type

init()

Creates a new accessibility technologies structure with an empy accessibility technology set.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- Sendable
- SetAlgebra

## See Also

### Supporting types

struct AccessibilityAttachmentModifier

A view modifier that adds accessibility properties to the view

