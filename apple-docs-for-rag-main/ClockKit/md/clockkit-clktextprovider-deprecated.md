

- ClockKit
-  CLKTextProvider Deprecated

Class

# CLKTextProvider

The common behavior for displaying text-based data in a complication.

watchOS 2.0–9.0Deprecated

``` source
class CLKTextProvider
```

Deprecated

Use WidgetKit to create complications for watchOS 10 or later. For more information, see Migrating to WidgetKit.

## Overview

Typically, you don’t create instances of this class yourself. Instead, you create instances of an appropriate subclass, based on the type of text data you’re trying to create. However, you can use the init(format:_:) initializer or textProviderWithFormat: class method to create a compound text provider constructed from a format string and the data from other text providers.

## Topics

### Creating a Compound Text Provider

convenience init(format: String, any CVarArg...)

Creates and returns a text provider built from the specified format string.

### Creating Localized Text Providers

class func localizableTextProvider(withStringsFileTextKey: String) -> Self

Creates a localizable simple text provider using the strings file key for the text.

class func localizableTextProvider(withStringsFileTextKey: String, shortTextKey: String?) -> Self

Creates a localizable simple text provider using strings file keys for both the regular text and the shorter fallback text.

class func localizableTextProvider(withStringsFileFormatKey: String, textProviders: [CLKTextProvider]) -> Self

Creates a localizable text provider with a strings file key that resolves to a format string, and with text providers for the replacement arguments.

### Setting the Tint Color

var tintColor: UIColor

The tint color to use for text.

### Supporting Accessibility

var accessibilityLabel: String?

A localized string that describes the text.

### Creating Empty Text Providers

init()

Creates an empty text provider.

class func new() -> Self

Creates an empty text provider.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CLKDateTextProvider
- CLKRelativeDateTextProvider
- CLKSimpleTextProvider
- CLKTimeIntervalTextProvider
- CLKTimeTextProvider

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Text providers

class CLKSimpleTextProvider

A single line of text to display in your complication interface.

Deprecated

class CLKDateTextProvider

A formatted string that conveys a date without any time information.

Deprecated

class CLKRelativeDateTextProvider

A formatted string that conveys the difference in time between the current date and a date that you specify.

Deprecated

class CLKTimeIntervalTextProvider

A formatted time range.

Deprecated

class CLKTimeTextProvider

A formatted time value.

Deprecated

