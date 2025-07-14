

- PHASE
- PHASESoundEventError
-  notFound 

Type Property

# notFound

An error the framework throws when it fails to find a particular sound event.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static var notFound: PHASESoundEventError.Code { get }
```

## See Also

### Identifying an Error Cause

static var apiMisuse: PHASESoundEventError.Code

An error that indicates the app misconfigures data or calls the framework in unsupported succession.

static var badData: PHASESoundEventError.Code

An error that indicates a sound event contains invalid data.

static var invalidInstance: PHASESoundEventError.Code

An error that indicates a sound event object is no longer valid.

static var outOfMemory: PHASESoundEventError.Code

An error the framework throws when a sound event depletes system memory.

static var systemNotInitialized: PHASESoundEventError.Code

An error the framework throws when engine initialization interrupts sound event playback.

