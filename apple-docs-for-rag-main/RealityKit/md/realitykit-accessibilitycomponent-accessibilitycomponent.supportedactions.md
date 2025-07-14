

- RealityKit
- AccessibilityComponent
-  AccessibilityComponent.SupportedActions 

Structure

# AccessibilityComponent.SupportedActions

A custom action that can be invoked on an entity in response to specific user cues.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS

``` source
struct SupportedActions
```

## Topics

### Initializers

init(rawValue: Int)

Creates a new option set from the given raw value.

### Instance Properties

let rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let activate: AccessibilityComponent.SupportedActions

Tells the entity to activate itself.

static let decrement: AccessibilityComponent.SupportedActions

Tells the entity to decrement the value of its content.

static let increment: AccessibilityComponent.SupportedActions

Tells the entity to increment the value of its content.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Accessibility

Improving the Accessibility of RealityKit Apps

Incorporate assistive technologies in your augmented reality app.

struct AccessibilityComponent

A component that stores accessibility information for an entity.

struct CustomContent

A CustomContent struct contains the accessibility strings for the labels you apply to your accessibility content.

enum RotorType

A context-sensitive event that helps VoiceOver users find the next instance of a related element.

enum AccessibilityEvents

