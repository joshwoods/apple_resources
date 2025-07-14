

- App Intents
-  AppShortcutPhraseToken 

Enumeration

# AppShortcutPhraseToken

Dynamic values you can include in the spoken phrases that run your shortcut.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum AppShortcutPhraseToken
```

## Topics

### Getting the tokens

case applicationName

### Operators

static func == (AppShortcutPhraseToken, AppShortcutPhraseToken) -> Bool

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

## See Also

### Creating a shortcut phrase

init(String)

init(stringLiteral: String)

Creates an instance initialized to the given string value.

init(stringInterpolation: AppShortcutPhrase&lt;Intent>.StringInterpolation)

Creates an instance from a string interpolation.

struct StringInterpolation

The type each segment of a string literal containing interpolations should be appended to.

