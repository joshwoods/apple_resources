

- RealityKit
- AccessibilityEvents
-  AccessibilityEvents.CustomAction 

Structure

# AccessibilityEvents.CustomAction

An accessibility event for a custom action defined in your app.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS

``` source
struct CustomAction
```

## Topics

### Initializers

init(key: LocalizedStringResource, entity: Entity)

### Instance Properties

var entity: Entity

The receiver of the action.

var key: LocalizedStringResource

The localized string key identifying this action.

## Relationships

### Conforms To

- Event
- Sendable

