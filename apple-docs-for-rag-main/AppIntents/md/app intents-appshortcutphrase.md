

- App Intents
-  AppShortcutPhrase 

Structure

# AppShortcutPhrase

A spoken phrase that causes the system to run the corresponding App Shortcut.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct AppShortcutPhrase where Intent : AppIntent
```

## Topics

### Creating a shortcut phrase

init(String)

init(stringLiteral: String)

Creates an instance initialized to the given string value.

init(stringInterpolation: AppShortcutPhrase&lt;Intent>.StringInterpolation)

Creates an instance from a string interpolation.

struct StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

enum AppShortcutPhraseToken

Dynamic values you can include in the spoken phrases that run your shortcut.

### Type Aliases

typealias ExtendedGraphemeClusterLiteralType

A type that represents an extended grapheme cluster literal.

typealias StringLiteralType

A type that represents a string literal.

typealias UnicodeScalarLiteralType

A type that represents a Unicode scalar literal.

### Default Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByStringLiteral Implementations

## Relationships

### Conforms To

- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral

## See Also

### App Shortcut definition

struct AppShortcut

A type that defines a preconfigured shortcut for a specific app intent.

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

