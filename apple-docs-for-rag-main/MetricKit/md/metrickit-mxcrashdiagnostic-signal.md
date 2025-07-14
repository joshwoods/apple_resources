

- MetricKit
- MXCrashDiagnostic
-  signal 

Instance Property

# signal

The signal associated with the crash.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
var signal: NSNumber? { get }
```

## Discussion

Processor-specific information is in the `usr/include/sys/signal.h` file in the SDK.

## See Also

### Viewing exception details

var exceptionType: NSNumber?

The Mach exception type of the crash.

var exceptionCode: NSNumber?

The encoded processor-specific information for the crash.

var exceptionReason: MXCrashDiagnosticObjectiveCExceptionReason?

var terminationReason: String?

The reason the app was terminated as a human-readable string.

var virtualMemoryRegionInfo: String?

Information about the region of memory an app accessed incorrectly, resulting in a bad-access crash.

