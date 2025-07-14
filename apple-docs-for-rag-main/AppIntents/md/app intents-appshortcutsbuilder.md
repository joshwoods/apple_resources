

- App Intents
-  AppShortcutsBuilder 

Enumeration

# AppShortcutsBuilder

A result builder that allows you to declaratively describe the App Shortcuts that your app provides.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@resultBuilder
enum AppShortcutsBuilder
```

## Topics

### Type Methods

static func buildBlock() -> [AppShortcut]

static func buildBlock(AppShortcut...) -> [AppShortcut]

static func buildBlock([AppShortcut]...) -> [AppShortcut]

static func buildExpression(AppShortcut) -> AppShortcut

static func buildExpression(AppShortcut) -> [AppShortcut]

static func buildLimitedAvailability([AppShortcut]) -> any _AppShortcutsContentMarker &amp; _LimitedAvailabilityAppShortcutsContentMarker

static func buildOptional((any _AppShortcutsContentEmitterMarker &amp; _AppShortcutsContentMarker &amp; _LimitedAvailabilityAppShortcutsContentMarker)?) -> [AppShortcut]

static func buildOptional((any _AppShortcutsContentMarker &amp; _LimitedAvailabilityAppShortcutsContentMarker)?) -> [AppShortcut]

## See Also

### App Shortcut definition

struct AppShortcut

A type that defines a preconfigured shortcut for a specific app intent.

struct AppShortcutPhrase

A spoken phrase that causes the system to run the corresponding App Shortcut.

struct NegativeAppShortcutPhrase

An object that represents a negative phrase.

struct NegativeAppShortcutPhrases

This is a set of negative phrases, which will all be added to the app-level negative training set. All the training data specified here, will be used to completely bypass your app

NSAppIconActionTintColorName

The tint color to apply to text and symbols in the App Shortcuts platter.

NSAppIconComplementingColorNames

The names of the colors to use for the background of the App Shortcuts platter.

enum ShortcutTileColor

Describes the colors a shortcut tile in the Shortcuts app.

