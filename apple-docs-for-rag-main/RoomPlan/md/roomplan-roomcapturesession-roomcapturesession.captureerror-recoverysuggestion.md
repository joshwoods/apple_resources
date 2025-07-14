

- RoomPlan
- RoomCaptureSession
- RoomCaptureSession.CaptureError
-  recoverySuggestion 

Instance Property

# recoverySuggestion

A localized message describing how one might recover from the failure.

RoomPlanFoundationiOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+watchOS 2.0+

``` source
var recoverySuggestion: String? { get }
```

## See Also

### Inspecting error information

var errorDescription: String?

A human-readable explanation for the error.

var failureReason: String?

A localized message describing the reason for the failure.

var helpAnchor: String?

A localized message providing “help” text if the user requests help.

var localizedDescription: String

Retrieve the localized description for this error.

