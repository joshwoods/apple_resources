

- Core Foundation
-  CFRunLoopRunResult 

Enumeration

# CFRunLoopRunResult

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFRunLoopRunResult
```

## Topics

### Constants

case finished

The running run loop mode has no sources or timers to process.

case handledSource

A source has been processed. This value is returned only if the run loop was told to run only until a source was processed.

case stopped

CFRunLoopStop(_:) was called on the run loop.

case timedOut

The specified time interval for running the run loop has passed.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Enumerations

struct CFFileSecurityClearOptions

struct CFISO8601DateFormatOptions

struct CFURLEnumeratorOptions

Options for controlling enumerator behavior.

enum CFURLEnumeratorResult

Result codes from the CFURLEnumeratorGetNextURL(_:_:_:) function.

enum CGRectEdge

