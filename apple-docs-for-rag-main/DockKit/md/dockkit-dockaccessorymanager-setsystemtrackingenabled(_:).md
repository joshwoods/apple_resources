

- DockKit
- DockAccessoryManager
-  setSystemTrackingEnabled(\_:) 

Instance Method

# setSystemTrackingEnabled(\_:)

Enable and disable system tracking for camera-enabled apps.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func setSystemTrackingEnabled(_ isEnabled: Bool) async throws
```

## Mentioned in 

Modify rotation and positioning programmatically

## Discussion

DockKit enables system tracking by default, and any camera stream automatically generates and sends tracking events when a device docks to a compatible dock accessory.

Always set this value to `false` before performing your own custom tracking.

Throws

DockKitError.notSupported if called on macOS.

## See Also

### Changing tracking behavior

var isSystemTrackingEnabled: Bool

An indication of whether system tracking is enabled.

