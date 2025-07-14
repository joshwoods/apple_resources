

- PHASE
-  PHASESoundEventError 

Structure

# PHASESoundEventError

A sound event error that PHASE reports.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct PHASESoundEventError
```

## Topics

### Creating an Error

enum Code

Codes that identify sound event errors.

### Identifying an Error Cause

static var apiMisuse: PHASESoundEventError.Code

An error that indicates the app misconfigures data or calls the framework in unsupported succession.

static var badData: PHASESoundEventError.Code

An error that indicates a sound event contains invalid data.

static var invalidInstance: PHASESoundEventError.Code

An error that indicates a sound event object is no longer valid.

static var notFound: PHASESoundEventError.Code

An error the framework throws when it fails to find a particular sound event.

static var outOfMemory: PHASESoundEventError.Code

An error the framework throws when a sound event depletes system memory.

static var systemNotInitialized: PHASESoundEventError.Code

An error the framework throws when engine initialization interrupts sound event playback.

### Type Properties

static var errorDomain: String

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Sound Event Errors

enum Code

Codes that identify sound event errors.

let PHASESoundEventErrorDomain: String

A unique error domain for sound events.

