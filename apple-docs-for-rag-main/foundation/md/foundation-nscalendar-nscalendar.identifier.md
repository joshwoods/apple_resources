

- Foundation
- NSCalendar
-  NSCalendar.Identifier 

Structure

# NSCalendar.Identifier

The supported calendar types.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Identifier
```

## Discussion

Use these identifiers to specify the kind of calendar. The Gregorian calendar is the calendar typically used in Europe, the Western Hemisphere, and elsewhere.

## Topics

### Initializers

init(String)

init(rawValue: String)

### Type Properties

static let gregorian: NSCalendar.Identifier

Identifier for the Gregorian calendar.

static let ISO8601: NSCalendar.Identifier

Identifier for the ISO8601 calendar.

static let buddhist: NSCalendar.Identifier

Identifier for the Buddhist calendar.

static let chinese: NSCalendar.Identifier

Identifier for the Chinese calendar.

static let coptic: NSCalendar.Identifier

Identifier for the Coptic calendar.

static let ethiopicAmeteAlem: NSCalendar.Identifier

Identifier for the Ethiopic (Amete Alem) calendar.

static let ethiopicAmeteMihret: NSCalendar.Identifier

Identifier for the Ethiopic (Amete Mihret) calendar.

static let hebrew: NSCalendar.Identifier

Identifier for the Hebrew calendar.

static let indian: NSCalendar.Identifier

Identifier for the Indian calendar.

static let islamic: NSCalendar.Identifier

Identifier for the Islamic calendar.

static let islamicCivil: NSCalendar.Identifier

Identifier for the Islamic civil calendar.

static let islamicTabular: NSCalendar.Identifier

Identifier for a tabular Islamic calendar.

static let islamicUmmAlQura: NSCalendar.Identifier

Identifier for the Islamic Umm al-Qura calendar.

static let japanese: NSCalendar.Identifier

Identifier for the Japanese calendar.

static let persian: NSCalendar.Identifier

Identifier for the Persian calendar.

static let republicOfChina: NSCalendar.Identifier

Identifier for the Republic of China calendar.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating and Initializing Calendars

init?(identifier: NSCalendar.Identifier)

Creates a new calendar specified by a given identifier.

init?(calendarIdentifier: NSCalendar.Identifier)

Initializes a calendar according to a given identifier.

