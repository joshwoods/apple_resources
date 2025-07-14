

- App Intents
-  NegativeAppShortcutPhrase 

Structure

# NegativeAppShortcutPhrase

An object that represents a negative phrase.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct NegativeAppShortcutPhrase
```

## Overview

Each negative phrase will be used to populate an app-level negative training set. This set will contain phrases that will completely bypass your app.

## Topics

### Structures

struct StringInterpolation

A string you construct using literal values, content from intent parameters, and other interpolated values.

### Initializers

init(String)

init(stringInterpolation: NegativeAppShortcutPhrase.StringInterpolation)

Creates an instance from a string interpolation.

init(stringLiteral: StringLiteralType)

Creates an instance initialized to the given string value.

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

struct AppShortcutPhrase

A spoken phrase that causes the system to run the corresponding App Shortcut.

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

