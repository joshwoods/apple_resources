

- Core Foundation
-  CFRunLoopMode 

Structure

# CFRunLoopMode

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFRunLoopMode
```

## Topics

### Type Properties

static let commonModes: CFRunLoopMode!

Objects added to a run loop using this value as the mode are monitored by all run loop modes that have been declared as a member of the set of “common” modes with CFRunLoopAddCommonMode(_:_:).

static let defaultMode: CFRunLoopMode!

Run loop mode that should be used when a thread is in its default, or idle, state, waiting for an event. This mode is used when the run loop is started with CFRunLoopRun().

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

struct CFNotificationName

struct CFNumberFormatterKey

struct CFStreamPropertyKey

typealias CFTypeRef

An untyped “generic” reference to any Core Foundation object.

