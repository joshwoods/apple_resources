

- WatchKit
-  WKExtendedRuntimeSessionErrorDomain 

Global Variable

# WKExtendedRuntimeSessionErrorDomain

The domain for errors reported by extended runtime sessions.

watchOS 6.0+

``` source
let WKExtendedRuntimeSessionErrorDomain: String
```

## Discussion

The session passes these errors to the session delegate’s extendedRuntimeSession(_:didInvalidateWith:error:) method.

## See Also

### Handling Errors

enum WKExtendedRuntimeSessionErrorCode

The error codes reported by extended runtime sessions.

