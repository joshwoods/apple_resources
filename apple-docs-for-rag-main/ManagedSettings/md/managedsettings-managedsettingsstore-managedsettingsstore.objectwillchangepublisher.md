

- ManagedSettings
- ManagedSettingsStore
-  ManagedSettingsStore.ObjectWillChangePublisher 

Type Alias

# ManagedSettingsStore.ObjectWillChangePublisher

The type of publisher that emits before the object has changed.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
typealias ObjectWillChangePublisher = ObservableObjectPublisher
```

## See Also

### Observing Current Settings

var objectWillChange: ObservableObjectPublisher

var $effectiveMaximumMovieRating: Published&lt;Int>.Publisher

The movie rating constraint that is active on this device.

var $effectiveMaximumTVShowRating: Published&lt;Int>.Publisher

The television show rating constraint that is active on this device.

