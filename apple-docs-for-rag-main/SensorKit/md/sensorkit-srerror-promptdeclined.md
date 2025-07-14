

- SensorKit
- SRError
-  promptDeclined 

Type Property

# promptDeclined

Occurs when the user cancels the sensor approval workflow.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
static var promptDeclined: SRError.Code { get }
```

## Discussion

The requestAuthorization(sensors:completion:) passes this error into the completion closure if the user declines the prompt by pressing Cancel. The framework also cancels the prompt if you call this function after the user had already responded to the prompt either by approving or denying access to the argument sensors.

## See Also

### Identifying an Error Cause

static var dataInaccessible: SRError.Code

Occurs when the app can’t access the sensor’s data.

static var fetchRequestInvalid: SRError.Code

Occurs when the app misconfigures a fetch request.

static var invalidEntitlement: SRError.Code

Occurs when the app lacks the required entitlement.

static var noAuthorization: SRError.Code

Occurs when the user declines sensor access in the Settings app.

