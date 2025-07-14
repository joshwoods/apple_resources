

- App Intents
-  AppShortcutOptionsCollectionProtocol 

Protocol

# AppShortcutOptionsCollectionProtocol

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol AppShortcutOptionsCollectionProtocol
```

## Topics

### Associated Types

associatedtype Provider : DynamicOptionsProvider

**Required**

### Instance Properties

var dynamicOptionsProvider: Self.Provider

**Required**

var systemImageName: String?

**Required**

var title: LocalizedStringResource

**Required**

## Relationships

### Conforming Types

- AppShortcutOptionsCollection

## See Also

### App Shortcut options

struct AppShortcutOptionsCollection

Represents a collection of options for parameters of an App Shortcut.

protocol AppShortcutOptionsCollectionSpecification

enum AppShortcutOptionsCollectionSpecificationBuilder

