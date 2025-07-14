

- FamilyControls
- AuthorizationCenter
-  AuthorizationCenter.ObjectWillChangePublisher 

Type Alias

# AuthorizationCenter.ObjectWillChangePublisher

The type of publisher that emits before the object has changed.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
typealias ObjectWillChangePublisher = ObservableObjectPublisher
```

## See Also

### Tracking Authorization Changes

var authorizationStatus: AuthorizationStatus

The status of your app’s authorization to provide parental controls.

var $authorizationStatus: Published&lt;AuthorizationStatus>.Publisher

A publisher for the authorization status property.

var objectWillChange: ObservableObjectPublisher

