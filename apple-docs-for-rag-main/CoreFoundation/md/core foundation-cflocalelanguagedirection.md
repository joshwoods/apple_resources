

- Core Foundation
-  CFLocaleLanguageDirection 

Enumeration

# CFLocaleLanguageDirection

These constants describe the text direction for a language. They are returned by the functions CFLocaleGetLanguageCharacterDirection(_:) and CFLocaleGetLanguageLineDirection(_:).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFLocaleLanguageDirection
```

## Topics

### Constants

case unknown

case leftToRight

case rightToLeft

case topToBottom

case bottomToTop

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

Locale Property Keys

Predefined locale keys used to get property values.

Locale Calendar Identifiers

Predefined locale keys used to get calendar values—values for `kCFLocaleCalendarIdentifier`.

Locale Change Notification

Identifier for notification sent if the current locale changes.

