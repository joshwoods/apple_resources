

- App Intents
-  AppShortcut 

Structure

# AppShortcut

A type that defines a preconfigured shortcut for a specific app intent.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct AppShortcut
```

## Mentioned in 

Creating your first app intent

## Overview

Related sessions from WWDC22

Session 10170: Implement App Shortcuts with App Intents, and session 10169: Design App Shortcuts.

Note

Apple may extract anonymized App Shortcuts data such as localized phrases, display representation values, and the title and description of related intents. Machine learning models use this data when training to help improve the App Shortcuts experience.

## Topics

### Creating an app shortcut

init&lt;Intent>(intent: Intent, phrases: [AppShortcutPhrase&lt;Intent>], shortTitle: LocalizedStringResource, systemImageName: String)

Initializes an App Shortcut with phrases that run the app intent, a title, and an image.

init&lt;Intent, Value, Parameter, ParameterKeyPath>(intent: Intent, phrases: [AppShortcutPhrase&lt;Intent>], shortTitle: LocalizedStringResource, systemImageName: String, parameterPresentation: AppShortcutParameterPresentation&lt;Intent, Value, Parameter, ParameterKeyPath>)

Initializes an App Shortcut with phrases that run the app intent, a title, an image, and specified parameters.

init&lt;Intent>(intent: Intent, phrases: [AppShortcutPhrase&lt;Intent>], shortTitle: LocalizedStringResource?, systemImageName: String?)

Initializes an App Shortcut with phrases that run the app intent, a title, and an image.

Deprecated

## See Also

### App Shortcut definition

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

enum AppShortcutsBuilder

A result builder that allows you to declaratively describe the App Shortcuts that your app provides.

enum ShortcutTileColor

Describes the colors a shortcut tile in the Shortcuts app.

