

- Core Foundation
-  CFURLEnumeratorResult 

Enumeration

# CFURLEnumeratorResult

Result codes from the CFURLEnumeratorGetNextURL(_:_:_:) function.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFURLEnumeratorResult
```

## Topics

### Constants

case success

The enumerator was advanced successfully and returned a valid URL.

case end

The enumeration is complete.

case error

An error occurred during enumeration. The `error` parameter of the function is populated with error information.

case directoryPostOrderSuccess

The recursive post-order enumerator returned the URL for a directory after having returned the URLs for all of the directory’s descendents.

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

### Enumerations

struct CFFileSecurityClearOptions

struct CFISO8601DateFormatOptions

enum CFRunLoopRunResult

struct CFURLEnumeratorOptions

Options for controlling enumerator behavior.

enum CGRectEdge

