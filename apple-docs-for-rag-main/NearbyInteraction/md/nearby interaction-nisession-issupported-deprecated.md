

- Nearby Interaction
- NISession
-  isSupported Deprecated

Type Property

# isSupported

A Boolean value that indicates whether the device supports basic interaction-session functionality.

iOS 14.0–16.0DeprecatediPadOS 14.0–16.0DeprecatedMac Catalyst 14.0–16.0DeprecatedwatchOS 7.3–9.0Deprecated

``` source
class var isSupported: Bool { get }
```

## Mentioned in 

Initiating and maintaining a session

## Discussion

Warning

This property is deprecated.

### Check the Device’s Supported Features

In iOS 16 and watchOS 9, check a device’s supported features with deviceCapabilities instead of calling this function.

The value of the supportsPreciseDistanceMeasurement device capability is equivalent to this property, as demonstrated in the following code.

```
var isSupported : Bool
if #available(iOS 16.0, watchOS 9.0, *) {
    isSupported = NISession.deviceCapabilities.supportsPreciseDistanceMeasurement
} else {
    isSupported = NISession.isSupported
}
if isSupported {
    // Initiate a nearby interaction session.
}
```

