

- Core Foundation
-  CFNotificationName 

Structure

# CFNotificationName

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFNotificationName
```

## Topics

### Type Properties

static let cfLocaleCurrentLocaleDidChange: CFNotificationName!

Identifier for the notification sent if the current locale changes.

static let cfTimeZoneSystemTimeZoneDidChange: CFNotificationName!

Name of the notification posted when the system time zone changes.

### Initializers

init(CFString)

init(rawValue: CFString)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Data Types

typealias CFAllocatorTypeID

struct CFCalendarIdentifier

struct CFDateFormatterKey

typealias CFErrorDomain

struct CFLocaleIdentifier

struct CFLocaleKey

struct CFNumberFormatterKey

struct CFRunLoopMode

struct CFStreamPropertyKey

typealias CFTypeRef

An untyped “generic” reference to any Core Foundation object.

