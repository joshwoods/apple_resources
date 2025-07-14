

- Core Media
- CMTimebase
-  CMTimebase.Error 

Structure

# CMTimebase.Error

Constants that describe timebase errors.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Error
```

## Topics

### Constants

static let allocationFailed: NSError

A timebase error that indicates the memory allocation fails.

static let invalidParameter: NSError

A timebase error that indicates a parameter isn’t valid.

static let missingRequiredParameter: NSError

A timebase error that indicates a missing parameter.

static let readOnly: NSError

A timebase error that indicates the system attempts to modify a read-only timebase.

static let timerIntervalTooShort: NSError

A timebase error that indicates the time interval is too short.

## Relationships

### Conforms To

- Sendable

## See Also

### Constants

struct NotificationKey

Constants that describe notification keys.

static var typeID: CFTypeID

A Core Foundation type identifier that represents a timebase object.

