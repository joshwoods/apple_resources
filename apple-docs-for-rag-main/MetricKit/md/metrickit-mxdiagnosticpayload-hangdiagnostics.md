

- MetricKit
- MXDiagnosticPayload
-  hangDiagnostics 

Instance Property

# hangDiagnostics

The diagnostic reports for times when the app was too busy to handle input responsively during the reporting period.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 12.0+visionOS 1.0+

``` source
var hangDiagnostics: [MXHangDiagnostic]? { get }
```

## See Also

### Reading responsiveness metrics

var appLaunchDiagnostics: [MXAppLaunchDiagnostic]?

The diagnostic reports for the app launch time.

