

- PHASE
- PHASESoundEventError
-  PHASESoundEventError.Code 

Enumeration

# PHASESoundEventError.Code

Codes that identify sound event errors.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
enum Code
```

## Topics

### Errors

case apiMisuse

An error that indicates the app misconfigures data or calls the framework in unsupported succession.

case badData

An error that indicates a sound event contains invalid data.

case invalidInstance

An error that indicates a sound event object is no longer valid.

case notFound

An error the framework throws when it fails to find a particular sound event.

case outOfMemory

An error the framework throws when a sound event depletes system memory.

case systemNotInitialized

An error the framework throws when engine initialization interrupts sound event playback.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Sound Event Errors

struct PHASESoundEventError

A sound event error that PHASE reports.

let PHASESoundEventErrorDomain: String

A unique error domain for sound events.

