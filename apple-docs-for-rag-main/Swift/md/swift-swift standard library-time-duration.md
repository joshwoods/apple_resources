

- Swift
- Swift Standard Library
-  Time 

API Collection

# Time

Measure how long an operation takes and determine schedules in the future.

## Topics

### Clocks

protocol Clock

A mechanism in which to measure time, and delay work until a given point in time.

struct ContinuousClock

A clock that measures time that always increments and does not stop incrementing while the system is asleep.

struct SuspendingClock

A clock that measures time that always increments but stops incrementing while the system is asleep.

### Durations

struct Duration

A representation of high precision time.

protocol DurationProtocol

A type that defines a duration for a given `InstantProtocol` type.

### Supporting Types

protocol InstantProtocol

## See Also

### Values and Collections

Numbers and Basic Values

Model data with numbers, Boolean values, and other fundamental types.

Strings and Text

Work with text using Unicode-safe strings.

Collections

Store and organize data using arrays, dictionaries, sets, and other data structures.

