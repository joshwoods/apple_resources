

- Core Location
- CLBeaconRegion
-  notifyEntryStateOnDisplay 

Instance Property

# notifyEntryStateOnDisplay

A Boolean value that indicates whether Core Location sends beacon notifications when the device’s display is on.

iOS 7.0–18.4DeprecatediPadOS 7.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.15–11.0Deprecated

``` source
var notifyEntryStateOnDisplay: Bool { get set }
```

## Discussion

When you set this to true, the location manager sends beacon notifications when the user turns on the display and the device is already inside the region. These are notifications the framework sends even if your app isn’t running. In that situation, the system launches your app into the background so that it can handle the notifications. In both situations, the location manager calls the locationManager(_:didDetermineState:for:) method of its delegate object.

The default value for this property is false.

