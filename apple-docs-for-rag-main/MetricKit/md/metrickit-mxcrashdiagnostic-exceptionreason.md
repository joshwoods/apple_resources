

- MetricKit
- MXCrashDiagnostic
-  exceptionReason 

Instance Property

# exceptionReason

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var exceptionReason: MXCrashDiagnosticObjectiveCExceptionReason? { get }
```

## See Also

### Viewing exception details

var exceptionType: NSNumber?

The Mach exception type of the crash.

var exceptionCode: NSNumber?

The encoded processor-specific information for the crash.

var signal: NSNumber?

The signal associated with the crash.

var terminationReason: String?

The reason the app was terminated as a human-readable string.

var virtualMemoryRegionInfo: String?

Information about the region of memory an app accessed incorrectly, resulting in a bad-access crash.

