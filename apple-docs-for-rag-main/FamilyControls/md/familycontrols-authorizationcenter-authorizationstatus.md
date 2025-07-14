

- FamilyControls
- AuthorizationCenter
-  authorizationStatus 

Instance Property

# authorizationStatus

The status of your app’s authorization to provide parental controls.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
@Published
var authorizationStatus: AuthorizationStatus { get }
```

## Discussion

The initial value is always AuthorizationStatus.notDetermined. The system sets this property only after a call to requestAuthorization(for:) succeeds. It then updates the property until a call to revokeAuthorization(completionHandler:) succeeds or your app exits.

To track changes to your app’s authorization status, attach a Subscriber to the `authorizationStatus` property.

```
let cancellable = center.$authorizationStatus
.sink() {
    switch center.authorizationStatus {
    case .notDetermined:
        // Handle the change to notDetermined.
    case .denied:
        // Handle the change to denied.
    case .approved:
        // Handle the change to approved.
   }
}
```

Alternatively, you can assign the AuthorizationCenter to an ObservedObject property inside a View. The system update the view whenever the status changes.

```
@ObservedObject var center = AuthorizationCenter.shared
```

The status may change due to external events, such as a child graduating to an adult account, or a parent or guardian changing the status in Settings.

Only access the `authorizationStatus` property on the main queue.

## See Also

### Tracking Authorization Changes

var $authorizationStatus: Published&lt;AuthorizationStatus>.Publisher

A publisher for the authorization status property.

var objectWillChange: ObservableObjectPublisher

typealias ObjectWillChangePublisher

The type of publisher that emits before the object has changed.

