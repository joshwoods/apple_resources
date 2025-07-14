

- Foundation
- Locale
-  Locale.Components 

Structure

# Locale.Components

A type that represents the components of a locale, for use when creating a locale with specific overrides.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Components
```

## Overview

Use Locale.Components with the init(components:) initializer to create a custom Locale that overrides specific traits of a default locale. When you create a locale with components, the locale uses any overridden values instead of defaults preferred by the region or language. Leave a property `nil` to accept the default value.

The properties in this type correspond with those in Locale, which declares them as read-only rather than read-write. You use this type to customize components when creating a custom locale, and use Locale to examine the components of an existing locale.

The following example creates a Locale.Components instance for US English, but then customizes its components. It sets the first day of the week to Monday and the hour cycle to zero-to-23. These components override the `en-US` defaults of Sunday and one-to-12, respectively. It then uses init(components:) to create a custom Locale.

```
var components = Locale.Components(languageCode: "en", languageRegion: "US")
components.firstDayOfWeek = Locale.Weekday.monday
components.hourCycle = Locale.HourCycle.zeroToTwentyThree
let locale = Locale(components: components)
```

## Topics

### Creating a locale components instance

init(identifier: String)

Creates a locale components instance with the specified identifier.

init(languageCode: Locale.LanguageCode?, script: Locale.Script?, languageRegion: Locale.Region?)

Creates a locale components instance with the specified language code, script, and region identifier.

init(locale: Locale)

Creates a language components instance from an existing locale.

### Specifying language components

var languageComponents: Locale.Language.Components

The Unicode language identifier part of a locale.

struct Components

A type that identifies a language by its various components.

### Specifying date and time components

var calendar: Calendar.Identifier?

The calendar used by the locale.

enum Identifier

An enumeration for the available calendars.

var firstDayOfWeek: Locale.Weekday?

The first day of the week as represented by this locale.

enum Weekday

A type that represents weekdays, used for indicating a locale’s first day of the week.

var hourCycle: Locale.HourCycle?

The hour cycle used by the locale, like one-to-twelve or zero-to-twenty-three.

enum HourCycle

A type that represents the hour cycle used in a locale, like one-to-twelve or zero-to-twenty-three.

var timeZone: TimeZone?

The time zone used by the locale.

### Specifiying measurement and counting components

var currency: Locale.Currency?

The currency used by the locale.

struct Currency

A type that represents the currency system used by a locale, like dollars or euros.

var measurementSystem: Locale.MeasurementSystem?

The measurement system used by the locale, like metric or the US system.

struct MeasurementSystem

A type that represents the measurement system used by a locale, like metric or the US system.

var numberingSystem: Locale.NumberingSystem?

The numbering system used by the locale.

struct NumberingSystem

A type that represents the numbering system used in a locale.

### Specifying region components

var region: Locale.Region?

The region used by the locale.

struct Region

A type that represents a geographic region, for use in specifying a locale or language.

var subdivision: Locale.Subdivision?

The optional subdivision of the region used by this locale.

struct Subdivision

A type that represents a subdivision of a region, such as a state in the US or a province in Canada.

var variant: Locale.Variant?

An optional variant used by the locale.

struct Variant

A type that represents a locale’s languate variant.

### Specifying ordering components

var collation: Locale.Collation?

The string sort order of the locale.

struct Collation

A type that represents the string sort order used by the locale.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a locale by components

init(components: Locale.Components)

Creates a locale from the given components.

init(languageCode: Locale.LanguageCode?, script: Locale.Script?, languageRegion: Locale.Region?)

Creates a locale with the specified language code, script, and region identifier.

init(languageComponents: Locale.Language.Components)

Creates a locale from the given language components.

struct Components

A type that identifies a language by its various components.

