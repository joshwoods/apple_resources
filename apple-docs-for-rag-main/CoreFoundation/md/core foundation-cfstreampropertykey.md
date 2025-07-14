

- Core Foundation
-  CFStreamPropertyKey 

Structure

# CFStreamPropertyKey

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFStreamPropertyKey
```

## Topics

### Type Properties

static let appendToFile: CFStreamPropertyKey!

Value is a `CFBoolean` value that indicates whether to append the written data to a file, if it already exists, rather than to replace its contents.

static let dataWritten: CFStreamPropertyKey!

Value is a `CFData` object that contains all the bytes written to a writable memory stream. You cannot modify this value.

static let fileCurrentOffset: CFStreamPropertyKey!

Value is a `CFNumber` object containing the current file offset.

static let socketNativeHandle: CFStreamPropertyKey!

Value is a `CFData` object that contains the native handle for a socket stream—of type CFSocketNativeHandle—to which the socket stream is connected.

static let socketRemoteHostName: CFStreamPropertyKey!

Value is a `CFString` object containing the name of the host to which the socket stream is connected or `NULL` if unknown.

static let socketRemotePortNumber: CFStreamPropertyKey!

Value is a `CFNumber` object containing the remote port number to which the socket stream is connected or `NULL` if unknown.

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

struct CFRunLoopMode

typealias CFTypeRef

An untyped “generic” reference to any Core Foundation object.

