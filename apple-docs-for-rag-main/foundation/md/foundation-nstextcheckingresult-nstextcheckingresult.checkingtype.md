

- Foundation
- NSTextCheckingResult
-  NSTextCheckingResult.CheckingType 

Structure

# NSTextCheckingResult.CheckingType

These constants specify the type of checking the methods should do. They are returned by resultType.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct CheckingType
```

## Topics

### Constants

static var orthography: NSTextCheckingResult.CheckingType

Attempts to identify the language

static var spelling: NSTextCheckingResult.CheckingType

Checks spelling.

static var grammar: NSTextCheckingResult.CheckingType

Checks grammar.

static var date: NSTextCheckingResult.CheckingType

Attempts to locate dates.

static var address: NSTextCheckingResult.CheckingType

Attempts to locate addresses.

static var link: NSTextCheckingResult.CheckingType

Attempts to locate URL links.

static var quote: NSTextCheckingResult.CheckingType

Replaces quotes with smart quotes.

static var dash: NSTextCheckingResult.CheckingType

Replaces dashes with em-dashes.

static var replacement: NSTextCheckingResult.CheckingType

Replaces characters such as (c) with the appropriate symbol (in this case ©).

static var correction: NSTextCheckingResult.CheckingType

Performs autocorrection on misspelled words.

static var regularExpression: NSTextCheckingResult.CheckingType

Matches a regular expression.

static var phoneNumber: NSTextCheckingResult.CheckingType

Matches a phone number.

static var transitInformation: NSTextCheckingResult.CheckingType

Matches a transit information, for example, flight information.

static var orthography: NSTextCheckingResult.CheckingType

Attempts to identify the language

static var spelling: NSTextCheckingResult.CheckingType

Checks spelling.

static var grammar: NSTextCheckingResult.CheckingType

Checks grammar.

static var date: NSTextCheckingResult.CheckingType

Attempts to locate dates.

static var address: NSTextCheckingResult.CheckingType

Attempts to locate addresses.

static var link: NSTextCheckingResult.CheckingType

Attempts to locate URL links.

static var quote: NSTextCheckingResult.CheckingType

Replaces quotes with smart quotes.

static var dash: NSTextCheckingResult.CheckingType

Replaces dashes with em-dashes.

static var replacement: NSTextCheckingResult.CheckingType

Replaces characters such as (c) with the appropriate symbol (in this case ©).

static var correction: NSTextCheckingResult.CheckingType

Performs autocorrection on misspelled words.

static var regularExpression: NSTextCheckingResult.CheckingType

Matches a regular expression.

static var phoneNumber: NSTextCheckingResult.CheckingType

Matches a phone number.

static var transitInformation: NSTextCheckingResult.CheckingType

Matches a transit information, for example, flight information.

### Initializers

init(rawValue: UInt64)

### Type Properties

static var allCustomTypes: NSTextCheckingResult.CheckingType

static var allSystemTypes: NSTextCheckingResult.CheckingType

static var allTypes: NSTextCheckingResult.CheckingType

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

Keys for Transit Components

The following constants identify the possible keys returned in the components dictionary.

Keys for Address Components

The following constants identify the possible keys returned in the addressComponents dictionary.

typealias NSTextCheckingTypes

Defines the types of checking that are available. These values can be combined using the C-bitwise OR operator. The system supports its own internal types, and the user can extend those types by subclassing `NSTextCheckingResult` and adding their own custom types.

struct NSTextCheckingKey

Anonymous

