

- SensorKit
- SRError
- SRError.Code
-  SRError.Code.noAuthorization 

Case

# SRError.Code.noAuthorization

Occurs when the user declines sensor access in the Settings app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
case noAuthorization
```

## Discussion

This error code indicates the user denied access for the sensor on the in-app prompt, or by switching off authorization for the sensor in Settings.

## See Also

### Errors

case promptDeclined

Occurs when the user cancels the sensor approval workflow.

case dataInaccessible

Occurs when the app can’t access the sensor’s data.

case fetchRequestInvalid

Occurs when the app misconfigures a fetch request.

case invalidEntitlement

Occurs when the app lacks the required entitlement.

