

- App Intents
-  AppShortcutOptionsCollection 

Structure

# AppShortcutOptionsCollection

Represents a collection of options for parameters of an App Shortcut.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct AppShortcutOptionsCollection where Provider : DynamicOptionsProvider
```

## Topics

### Initializers

init(Provider, title: LocalizedStringResource, systemImageName: String?)

Initializes a collection of options for App Shortcuts with the specified parameters.

### Instance Properties

let dynamicOptionsProvider: Provider

let systemImageName: String?

let title: LocalizedStringResource

## Relationships

### Conforms To

- AppShortcutOptionsCollectionProtocol

## See Also

### App Shortcut options

protocol AppShortcutOptionsCollectionProtocol

protocol AppShortcutOptionsCollectionSpecification

enum AppShortcutOptionsCollectionSpecificationBuilder

