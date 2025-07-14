

- MetricKit
- MXCrashDiagnostic
-  exceptionType 

Instance Property

# exceptionType

The Mach exception type of the crash.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
var exceptionType: NSNumber? { get }
```

## Discussion

Mach exception types are in the `usr/include/mach/exception_types.h` file in the SDK.

## See Also

### Viewing exception details

var exceptionCode: NSNumber?

The encoded processor-specific information for the crash.

var signal: NSNumber?

The signal associated with the crash.

var exceptionReason: MXCrashDiagnosticObjectiveCExceptionReason?

var terminationReason: String?

The reason the app was terminated as a human-readable string.

var virtualMemoryRegionInfo: String?

Information about the region of memory an app accessed incorrectly, resulting in a bad-access crash.

