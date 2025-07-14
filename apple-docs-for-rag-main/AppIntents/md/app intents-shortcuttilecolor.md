

- App Intents
-  ShortcutTileColor 

Enumeration

# ShortcutTileColor

Describes the colors a shortcut tile in the Shortcuts app.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum ShortcutTileColor
```

## Topics

### Getting the tile colors

case blue

A blue color.

case grape

A grape color.

case grayBlue

A grayish-blue color.

case grayBrown

A grayish-brown color.

case grayGreen

A grayish-green color.

case lightBlue

A light blue color.

case lime

A lime color.

case navy

A navy blue color.

case orange

An orange color.

case pink

A pink color.

case purple

A purple color.

case red

A red color.

case tangerine

A tangerine color.

case teal

A teal color.

case yellow

A yellow color.

### Operators

static func == (ShortcutTileColor, ShortcutTileColor) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

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

enum AppShortcutsBuilder

A result builder that allows you to declaratively describe the App Shortcuts that your app provides.

