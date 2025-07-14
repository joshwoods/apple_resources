

- Foundation
-  LocalizedStringResource 

Structure

# LocalizedStringResource

A reference to a localizable string, accessible from another process.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct LocalizedStringResource
```

## Overview

Use LocalizedStringResource to provide localizable strings with lookups you defer to a later time.

When you create a localized string or a localized attributed string with an initializer that takes String.LocalizationValue, those initializers lookup the localized string immediately. If you want to perform the lookup at a later time, use this LocalizedStringResource type to refer to the localizable strings. Then, when you need to perform localization, create a String or AttributedString from an initializer that takes a LocalizedStringResource parameter, such as:

- String: init(localized:) or init(localized:options:).

- AttributedString: init(localized:), init(localized:including:), or init(localized:including:).

This approach allows you to provide localizable strings to an entirely separate process, which may use a different locale. For example, consider an app with a data model type called `UserAction` that uses LocalizedStringResource rather than strings for its `title` and `description` properties.

```
public protocol UserAction {
    static var title: LocalizedStringResource { get }
    static var description: LocalizedStringResource { get }
}
```

This app (or one of its embedded frameworks) then uses these LocalizedStringResource members to defer looking up localized strings. Typically, this happens when calling out to another process over XPC.

```
public func perform(action: UserAction) {
    ...
    // Send text to another process via XPC or similar.
    performActionOutOfProcess(title: action.title, description: action.description)
}
```

Then, when the other process receives the call, it can alter the locale in the LocalizedStringResource, prior to resolving the localized strings.

```
func performActionOutOfProcess(title: LocalizedStringResource,
                               description: LocalizedStringResource) {
    // Set resource locales to match the current locale
    // of the separate process.
    var fixedTitle = title
    fixedTitle.locale = .current
    var fixedDescription = description
    fixedDescription.locale = .current

    // Look up localized strings.
    let titleString = String(localized: fixedTitle)
    let descriptionString = String(localized: fixedDescription)

    // Use a correctly localized title/description.
}
```

The App Intents framework uses LocalizedStringResource to perform a late resolution of localized strings. This allows the Siri UI to potentially use different localization preferences than the app providing the intent.

## Topics

### Creating a localized string resource

init(String.LocalizationValue, table: String?, locale: Locale, bundle: LocalizedStringResource.BundleDescription, comment: StaticString?)

Creates a localized string resource from a localization key and its bundle properties.

init(StaticString, defaultValue: String.LocalizationValue, table: String?, locale: Locale, bundle: LocalizedStringResource.BundleDescription, comment: StaticString?)

Creates a localized string resource from a static string and its bundle properties.

### Accessing resource properties

let key: String

The key to use to look up a localized string.

let defaultValue: String.LocalizationValue

The resource’s default value.

let table: String?

The name of the table containing the key-value pairs.

var bundle: LocalizedStringResource.BundleDescription

The bundle containing the table’s strings file.

enum BundleDescription

The location of a bundle to use for looking up localized strings, such as the main bundle, or a bundle at a specific file URL.

var locale: Locale

The locale to use to look up the localized string from the string resource.

## Relationships

### Conforms To

- CustomLocalizedStringResourceConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByStringInterpolation
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Sendable

## See Also

### Localization

struct Locale

Information about linguistic, cultural, and technological conventions for use in formatting data for presentation.

class NSOrthography

A description of the linguistic content of natural language text, typically used for spelling and grammar checking.

func NSLocalizedString(String, tableName: String?, bundle: Bundle, value: String, comment: String) -> String

Returns a localized string from a table that Xcode generates for you when exporting localizations.

protocol CustomLocalizedStringResourceConvertible

A type that provides an out-of-process localizable description.

struct URLResource

A resource located at a particular file URL within a bundle.

