

- ARKit
- ARKitSession
- ARKitSession.Error
-  dataProvider 

Instance Property

# dataProvider

The data provider that caused an error in a session.

visionOS 1.0+

``` source
let dataProvider: (any DataProvider)?
```

## See Also

### Inspecting ARKit errors

var code: ARKitSession.Error.Code

The error code for an ARKit session error.

enum Code

The error codes for ARKit sessions.

var errorDescription: String?

A localized message that describes the error that occurred.

