

- Foundation
- AttributedString
-  AttributedString.FormattingOptions 

Structure

# AttributedString.FormattingOptions

Options that affect the handling of attributes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct FormattingOptions
```

## Topics

### Creating Formatting Options

init()

Creates an empty attributed string.

init(NSAttributedString)

Creates a value-type attributed string from a reference type.

init(AttributedSubstring)

Creates an attributed string from an attributed substring.

### Using Defined Formatting Options

static let applyReplacementIndexAttribute: AttributedString.FormattingOptions

An option to add an attribute that marks replacements in localized strings.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Creating a Localized Attributed String

init(localized: String.LocalizationValue, options: AttributedString.FormattingOptions, table: String?, bundle: Bundle?, locale: Locale?, comment: StaticString?)

Creates an attributed string by looking up a localized string from the app’s bundle.

init&lt;S>(localized: String.LocalizationValue, options: AttributedString.FormattingOptions, table: String?, bundle: Bundle?, locale: Locale?, comment: StaticString?, including: S.Type)

Creates an attributed string by looking up a localized string from the app’s bundle, including an attribute scope.

init&lt;S>(localized: String.LocalizationValue, options: AttributedString.FormattingOptions, table: String?, bundle: Bundle?, locale: Locale?, comment: StaticString?, including: KeyPath&lt;AttributeScopes, S.Type>)

Creates an attributed string by looking up a localized string from the app’s bundle, including an attribute scope that a key path identifies.

struct LocalizationValue

A reference to a localizable string, with optional string interpolation.

init(localized: LocalizedStringResource)

Creates a localized attributed string from a localized string resource.

init&lt;S>(localized: LocalizedStringResource, including: S.Type)

Creates a localized attributed string from a localized string resource, including an attribute scope.

init&lt;S>(localized: LocalizedStringResource, including: KeyPath&lt;AttributeScopes, S.Type>)

Creates a localized attributed string from a localized string resource, including an attribute scope that a key path identifies.

struct LocalizedStringResource

A reference to a localizable string, accessible from another process.

