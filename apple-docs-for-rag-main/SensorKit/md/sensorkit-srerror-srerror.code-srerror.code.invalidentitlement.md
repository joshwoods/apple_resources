

- SensorKit
- SRError
- SRError.Code
-  SRError.Code.invalidEntitlement 

Case

# SRError.Code.invalidEntitlement

Occurs when the app lacks the required entitlement.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case invalidEntitlement
```

## Discussion

To allow the app to read sensor data, the system requires that the app’s code signature contain a special entitlement. For more information, see Configuring your project for sensor reading.

## See Also

### Errors

case promptDeclined

Occurs when the user cancels the sensor approval workflow.

case dataInaccessible

Occurs when the app can’t access the sensor’s data.

case fetchRequestInvalid

Occurs when the app misconfigures a fetch request.

case noAuthorization

Occurs when the user declines sensor access in the Settings app.

