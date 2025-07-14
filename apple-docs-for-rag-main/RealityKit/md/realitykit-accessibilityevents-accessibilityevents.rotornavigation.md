

- RealityKit
- AccessibilityEvents
-  AccessibilityEvents.RotorNavigation 

Structure

# AccessibilityEvents.RotorNavigation

An accessibility event associated with a rotor navigation.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS

``` source
@MainActor @preconcurrency
struct RotorNavigation
```

## Topics

### Initializers

init(rotorType: AccessibilityComponent.RotorType, hostEntity: Entity, currentItem: Any?, searchDirection: UIAccessibilityCustomRotor.Direction, resultHandler: (Any) -> Void)

### Instance Properties

let currentItem: Any?

The current element of the search.

let hostEntity: Entity

The entity containing the component declaring support for this rotor type.

let resultHandler: (Any) -> Void

The handler for the result of the current search. When observing RotorNavigation events

let rotorType: AccessibilityComponent.RotorType

The type of the rotor associated with the event.

let searchDirection: UIAccessibilityCustomRotor.Direction

The direction in which to search.

## Relationships

### Conforms To

- Event
- Sendable

