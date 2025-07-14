

- ARKit
- ARKitSession
- ARKitSession.Error
-  code 

Instance Property

# code

The error code for an ARKit session error.

visionOS 1.0+

``` source
var code: ARKitSession.Error.Code { get }
```

## See Also

### Inspecting ARKit errors

let dataProvider: (any DataProvider)?

The data provider that caused an error in a session.

enum Code

The error codes for ARKit sessions.

var errorDescription: String?

A localized message that describes the error that occurred.

