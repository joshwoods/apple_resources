

- FamilyControls
- AuthorizationCenter
-  objectWillChange 

Instance Property

# objectWillChange

FamilyControlsCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
var objectWillChange: ObservableObjectPublisher { get }
```

Available when `ObjectWillChangePublisher` is `ObservableObjectPublisher`.

## See Also

### Tracking Authorization Changes

var authorizationStatus: AuthorizationStatus

The status of your app’s authorization to provide parental controls.

var $authorizationStatus: Published&lt;AuthorizationStatus>.Publisher

A publisher for the authorization status property.

typealias ObjectWillChangePublisher

The type of publisher that emits before the object has changed.

