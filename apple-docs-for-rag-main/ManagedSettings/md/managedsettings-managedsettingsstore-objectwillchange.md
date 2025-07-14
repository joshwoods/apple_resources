

- ManagedSettings
- ManagedSettingsStore
-  objectWillChange 

Instance Property

# objectWillChange

ManagedSettingsCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
var objectWillChange: ObservableObjectPublisher { get }
```

Available when `ObjectWillChangePublisher` is `ObservableObjectPublisher`.

## See Also

### Observing Current Settings

var $effectiveMaximumMovieRating: Published&lt;Int>.Publisher

The movie rating constraint that is active on this device.

var $effectiveMaximumTVShowRating: Published&lt;Int>.Publisher

The television show rating constraint that is active on this device.

typealias ObjectWillChangePublisher

The type of publisher that emits before the object has changed.

