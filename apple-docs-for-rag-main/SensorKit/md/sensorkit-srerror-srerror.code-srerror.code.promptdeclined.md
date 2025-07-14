

- SensorKit
- SRError
- SRError.Code
-  SRError.Code.promptDeclined 

Case

# SRError.Code.promptDeclined

Occurs when the user cancels the sensor approval workflow.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case promptDeclined
```

## Discussion

The requestAuthorization(sensors:completion:) passes this error into the completion closure if the user declines the prompt by pressing Cancel. The framework also cancels the prompt if you call this function after the user had already responded to the prompt either by approving or denying access to the argument sensors.

## See Also

### Errors

case dataInaccessible

Occurs when the app can’t access the sensor’s data.

case fetchRequestInvalid

Occurs when the app misconfigures a fetch request.

case invalidEntitlement

Occurs when the app lacks the required entitlement.

case noAuthorization

Occurs when the user declines sensor access in the Settings app.

