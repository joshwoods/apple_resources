

- RealityKit
- AccessibilityEvents
- AccessibilityEvents.RotorNavigation
-  init(rotorType:hostEntity:currentItem:searchDirection:resultHandler:) 

Initializer

# init(rotorType:hostEntity:currentItem:searchDirection:resultHandler:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS

``` source
@MainActor @preconcurrency
init(
    rotorType: AccessibilityComponent.RotorType,
    hostEntity: Entity,
    currentItem: Any?,
    searchDirection: UIAccessibilityCustomRotor.Direction,
    resultHandler: @escaping (Any) -> Void
)
```

