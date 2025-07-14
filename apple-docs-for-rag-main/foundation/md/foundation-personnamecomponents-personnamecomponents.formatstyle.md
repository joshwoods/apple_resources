

- Foundation
- PersonNameComponents
-  PersonNameComponents.FormatStyle 

Structure

# PersonNameComponents.FormatStyle

A type used to format a person’s name with a style appropriate for the given locale.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct FormatStyle
```

## Overview

Personal names deserve careful and respectful treatment in your apps. Each locale has its own set of rules and conventions to construct and represent personal names. These rules vary widely across different locales in several ways, including the sort and display order of given and family names, the use of salutations and honorifics, and other concerns related to the grammar, spelling, punctuation, and formatting.

A `PersonNameComponents.FormatStyle` creates human readable text from an instance of PersonNameComponents. You can customize the formatting using the style and locale properties. The system automatically caches instances with unique configurations of the format style to enhance performance.

### Format Styles

You can configure a `PersonNameComponents.FormatStyle` to represent names in a variety of styles:

- Long (PersonNameComponents.FormatStyle.Style.long)

- Medium (PersonNameComponents.FormatStyle.Style.medium)

- Short (PersonNameComponents.FormatStyle.Style.short)

- Abbreviated (PersonNameComponents.FormatStyle.Style.abbreviated)

When determining how to represent a name in a particular style, a number of factors determine the final format. In order of priority:

1.  Script derived behaviors — Scripts may specify a strict sort or display order of given and family names, and the availability of styles. The format style assigns an “Unknown” script, which has its own set of behaviors and characteristics, to a name that contains more than one script (for example, given name: John; family name: 王).

2.  User specified preferences — Users can enable and configure the display of short names, as well as whether to display nicknames when available. Users can also override the default sort and display order of given and family names for their current locale.

3.  Locale derived defaults — Locales specify a default sort and display order for given and family names.

4.  Developer specified configuration — The style property value set for the `PersonNameComponent.FormatStyle`.

In the case of a conflict, the format style uses the factor with the highest precedence. For example, the U.S. English (`en-US`) style formats names in “given name followed by the family name” (for example, Anne Johnson). This behavior would be overridden if the user changed their system preferences to have names displayed as family name followed by given name (for example, Johnson, Anne), because user-specified preferences take precedence over locale-derived defaults. Furthermore, if the name to be formatted were Japanese (for example, given name: 泰夫; family name: 木田), the behavior derived for the name’s script (CJK, for Chinese, Japanese, and Korean languages) would take precedence over any locale-derived defaults or user-specified preferences to have the name displayed as family name followed by given name (for example, 木田 泰夫).

These considerations extend to the availability of certain format styles as well. Because developer-specified configurations have the lowest precedence, the value set for the formatter’s style property is invalidated if it isn’t supported for the locale, user preferences, or script. If the specified style isn’t available, it uses the next longest valid style. For example, a name in Arabic script (for example, أحمد الراجحي) doesn’t support the Abbreviated style, so it uses the Short style instead.

For more information and examples, see style.

### Formatting Person Name Components

Use either formatted() or formatted(_:), both instance methods of PersonNameComponents, to create a string representation of a name.

The formatted() method to applies the default format style to a name. For example:

```
var tlc = PersonNameComponents()
tlc.familyName = "Clark"
tlc.givenName = "Thomas"
tlc.middleName = "Louis"
tlc.namePrefix = "Dr."
tlc.nickname = "Tom"
tlc.nameSuffix = "Esq."

tlc.formatted()
// Thomas Clark
```

The formatted(_:) method applies a custom format style to a name. You can use the static factory method `name(style:)-6tpu3` to create a custom format style as a parameter to the method. For example:

```
tlc.formatted(.name(style: .long))
// Dr. Thomas Louis Clark Esq.

tlc.formatted(.name(style: .medium))
// Thomas Clark

tlc.formatted(.name(style: .short))
// Tom

tlc.formatted(.name(style: .abbreviated))
// TC
```

You can create and reuse a format style instance to format multiple names. For example:

```
let customPersonFormatStyle = PersonNameComponents.FormatStyle(style: .medium, locale: Locale(identifier: "en_US"))

tlc.formatted(customPersonFormatStyle)
// Thomas Clark

mlr.formatted(customPersonFormatStyle)
// Maria Ruiz
```

## Topics

### Creating a Format Style

init(style: PersonNameComponents.FormatStyle.Style, locale: Locale)

Creates an instance using the provided format style and locale.

### Parsing Person Name Components

init(String) throws

Creates a person name components object from a given string.

init&lt;S>(S.ParseInput, strategy: S) throws

Creates a person name components object from a given string by applying the provided parsing strategy.

### Modifying a Format Style

var style: PersonNameComponents.FormatStyle.Style

Specifies the style of the formatted result.

enum Style

The type that represents the style of the formatted result.

var locale: Locale

The locale to use when formatting the person name components.

var attributed: PersonNameComponents.AttributedStyle

The style used to create a locale-aware attributed string representation of an instance of person name components.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- FormatStyle
- Hashable
- ParseableFormatStyle
- Sendable

## See Also

### Formatting Person Name Components

func formatted() -> String

Generates a locale-aware string representation of an instance of person name components using the default format style.

func formatted&lt;S>(S) -> S.FormatOutput

Generates a locale-aware string representation of an instance of person name components using the provided format style.

