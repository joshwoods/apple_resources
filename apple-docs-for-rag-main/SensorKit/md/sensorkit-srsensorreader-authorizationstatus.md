

- SensorKit
- SRSensorReader
-  authorizationStatus 

Instance Property

# authorizationStatus

The status of the user’s agreement to let the app access this reader’s sensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
var authorizationStatus: SRAuthorizationStatus { get }
```

## Discussion

When an app wishes to read data from a particular sensor, it checks for user approval first by accessing the value of this property. If the value is SRAuthorizationStatus.authorized, an app may begin recording (see startRecording()) and execute data fetches (see fetch(_:)).

If the value is SRAuthorizationStatus.denied, an app can’t begin recording or execute fetches until the user switches on authorization for the reader’s sensor in Settings.

If the value is SRAuthorizationStatus.notDetermined, the user has not answered the in-app prompt. To display the prompt, call requestAuthorization(sensors:completion:).

## See Also

### Checking user authorization

class func requestAuthorization(sensors: Set&lt;SRSensor>, completion: ((any Error)?) -> Void)

Requests user permission to read one or more sensors.

enum SRAuthorizationStatus

The states that model whether the user approves the app to read a particular sensor.

