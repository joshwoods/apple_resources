

- App Intents
-  NegativeAppShortcutPhrases 

Structure

# NegativeAppShortcutPhrases

This is a set of negative phrases, which will all be added to the app-level negative training set. All the training data specified here, will be used to completely bypass your app

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct NegativeAppShortcutPhrases
```

## Topics

### Initializers

init(phrases: [NegativeAppShortcutPhrase])

## See Also

### App Shortcut definition

struct AppShortcut

A type that defines a preconfigured shortcut for a specific app intent.

struct AppShortcutPhrase

A spoken phrase that causes the system to run the corresponding App Shortcut.

struct NegativeAppShortcutPhrase

An object that represents a negative phrase.

NSAppIconActionTintColorName

The tint color to apply to text and symbols in the App Shortcuts platter.

NSAppIconComplementingColorNames

The names of the colors to use for the background of the App Shortcuts platter.

enum AppShortcutsBuilder

A result builder that allows you to declaratively describe the App Shortcuts that your app provides.

enum ShortcutTileColor

Describes the colors a shortcut tile in the Shortcuts app.

