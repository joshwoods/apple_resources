

- SwiftUI
-  LocalizedStringKey 

Structure

# LocalizedStringKey

The key used to look up an entry in a strings file or strings dictionary file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct LocalizedStringKey
```

## Mentioned in 

Adding a search interface to your app

Preparing views for localization

## Overview

Initializers for several SwiftUI types – such as Text, Toggle, Picker and others – implicitly look up a localized string when you provide a string literal. When you use the initializer `Text("Hello")`, SwiftUI creates a `LocalizedStringKey` for you and uses that to look up a localization of the `Hello` string. This works because `LocalizedStringKey` conforms to ExpressibleByStringLiteral.

Types whose initializers take a `LocalizedStringKey` usually have a corresponding initializer that accepts a parameter that conforms to StringProtocol. Passing a `String` variable to these initializers avoids localization, which is usually appropriate when the variable contains a user-provided value.

As a general rule, use a string literal argument when you want localization, and a string variable argument when you don’t. In the case where you want to localize the value of a string variable, use the string to create a new `LocalizedStringKey` instance.

The following example shows how to create Text instances both with and without localization. The title parameter provided to the Section is a literal string, so SwiftUI creates a `LocalizedStringKey` for it. However, the string entries in the `messageStore.today` array are `String` variables, so the Text views in the list use the string values verbatim.

```
List {
    Section(header: Text("Today")) {
        ForEach(messageStore.today) { message in
            Text(message.title)
        }
    }
}
```

If the app is localized into Japanese with the following translation of its `Localizable.strings` file:

```
"Today" = "今日";
```

When run in Japanese, the example produces a list like the following, localizing “Today” for the section header, but not the list items.

## Topics

### Creating a key from a literal value

init(String)

Creates a localized string key from the given string value.

init(stringLiteral: String)

Creates a localized string key from the given string literal.

### Creating a key from an interpolation

init(stringInterpolation: LocalizedStringKey.StringInterpolation)

Creates a localized string key from the given string interpolation.

struct StringInterpolation

Represents the contents of a string literal with interpolations while it’s being built, for use in creating a localized string key.

## Relationships

### Conforms To

- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral

## See Also

### Localizing text

Preparing views for localization

Specify hints and add strings to localize your SwiftUI views.

var locale: Locale

The current locale that views should use.

func typesettingLanguage(_:isEnabled:)

Specifies the language for typesetting.

struct TypesettingLanguage

Defines how typesetting language is determined for text.

