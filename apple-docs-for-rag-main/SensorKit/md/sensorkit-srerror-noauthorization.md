

- SensorKit
- SRError
-  noAuthorization 

Type Property

# noAuthorization

Occurs when the user declines sensor access in the Settings app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static var noAuthorization: SRError.Code { get }
```

## See Also

### Identifying an Error Cause

static var promptDeclined: SRError.Code

Occurs when the user cancels the sensor approval workflow.

static var dataInaccessible: SRError.Code

Occurs when the app can’t access the sensor’s data.

static var fetchRequestInvalid: SRError.Code

Occurs when the app misconfigures a fetch request.

static var invalidEntitlement: SRError.Code

Occurs when the app lacks the required entitlement.

