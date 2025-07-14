

- SensorKit
- SRSensorReader
-  requestAuthorization(sensors:completion:) 

Type Method

# requestAuthorization(sensors:completion:)

Requests user permission to read one or more sensors.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class func requestAuthorization(
    sensors: Set,
    completion: @escaping ((any Error)?) -> Void
)
```

``` source
class func requestAuthorization(sensors: Set) async throws
```

## Parameters 

`sensors`  

One or more sensors your app requests.

`completion`  

A closure to run after the framework determines user authorization.

## Discussion

Concurrency Note

In Swift, you can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func requestAuthorization(sensors: Set) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Call this function for sensors in which authorizationStatus is SRAuthorizationStatus.notDetermined to display a prompt that requests user authorization. When the prompt dismisses, the framework calls the `completion` closure. Your delegate needs to wait for a call to sensorReader(_:didChange:) to determine whether the user approves sensor access.

If you pass a sensor into this function for which the user already answered the in-app prompt, the framework cancels the prompt with SRError.Code.promptDeclined. When the user has already answered the prompt for a particular sensor, its authorizationStatus is SRAuthorizationStatus.authorized or SRAuthorizationStatus.denied. The user may change the authorization status for a sensor in Settings \> Privacy \> Research Sensor & Usage Data.

For more information about the authorization workflow, see Configuring your project for sensor reading.

## See Also

### Checking user authorization

var authorizationStatus: SRAuthorizationStatus

The status of the user’s agreement to let the app access this reader’s sensor.

enum SRAuthorizationStatus

The states that model whether the user approves the app to read a particular sensor.

