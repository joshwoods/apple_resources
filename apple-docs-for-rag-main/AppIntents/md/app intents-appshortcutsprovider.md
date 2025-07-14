

- App Intents
-  AppShortcutsProvider 

Protocol

# AppShortcutsProvider

A type alias for the type that provides an app’s preconfigured shortcuts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol AppShortcutsProvider
```

## Mentioned in 

Creating your first app intent

## Overview

Related sessions from WWDC22

Session 10170: Implement App Shortcuts with App Intents, and session 10169: Design App Shortcuts.

Note

Apple may extract anonymized App Shortcuts data such as localized phrases, display representation values, and the title and description of related intents. Machine learning models use this data when training to help improve the App Shortcuts experience.

## Topics

### Providing App Shortcuts

static var appShortcuts: [AppShortcut]

**Required**

enum AppShortcutsBuilder

A result builder that allows you to declaratively describe the App Shortcuts that your app provides.

### Configuring shortcut tiles

static var shortcutTileColor: ShortcutTileColor

The background color of the tile that Shortcuts displays for each of the app’s App Shortcuts.

**Required** Default implementation provided.

enum ShortcutTileColor

Describes the colors a shortcut tile in the Shortcuts app.

### Updating stored parameters

static func updateAppShortcutParameters()

### Type Aliases

typealias OptionsCollection

typealias ParameterPresentation

typealias Summary

typealias TitleDeprecated

### Type Properties

static var negativePhrases: NegativeAppShortcutPhrases

