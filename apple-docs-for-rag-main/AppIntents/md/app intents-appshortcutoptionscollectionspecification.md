

- App Intents
-  AppShortcutOptionsCollectionSpecification 

Protocol

# AppShortcutOptionsCollectionSpecification

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol AppShortcutOptionsCollectionSpecification : Sendable, Sequence where Self.Element == any AppShortcutOptionsCollectionProtocol
```

## Topics

### Associated Types

associatedtype Value : _IntentValue

**Required**

## Relationships

### Inherits From

- Sendable
- Sequence

## See Also

### App Shortcut options

struct AppShortcutOptionsCollection

Represents a collection of options for parameters of an App Shortcut.

protocol AppShortcutOptionsCollectionProtocol

enum AppShortcutOptionsCollectionSpecificationBuilder

