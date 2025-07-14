

- DockKit
- DockAccessoryManager
-  isSystemTrackingEnabled 

Instance Property

# isSystemTrackingEnabled

An indication of whether system tracking is enabled.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var isSystemTrackingEnabled: Bool { get }
```

## Discussion

This property is `true` if system tracking is enabled; otherwise the property is `false`. To change system tracking behavior, see setSystemTrackingEnabled(_:).

## See Also

### Changing tracking behavior

func setSystemTrackingEnabled(Bool) async throws

Enable and disable system tracking for camera-enabled apps.

