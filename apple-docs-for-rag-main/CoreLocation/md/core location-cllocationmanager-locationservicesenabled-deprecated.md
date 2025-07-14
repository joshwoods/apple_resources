

- Core Location
- CLLocationManager
-  locationServicesEnabled Deprecated

Instance Property

# locationServicesEnabled

A Boolean value indicating whether location services are enabled on the device.

macOS 10.15–10.15Deprecated

``` source
var locationServicesEnabled: Bool { get }
```

Deprecated

Use the locationServicesEnabled() class method instead.

## Discussion

In iOS, the user can enable or disable location services using the controls in Settings \> Location Services. In macOS, the user can enable or disable location services from the Security & Privacy system preference.

If this property contains the value false and you start location updates anyway, the Core Location framework prompts the user with a confirmation alert asking whether location services should be reenabled.

### Special Considerations

In iOS, this property is declared as `nonatomic`. In macOS, it is declared as `atomic`.

## See Also

### Properties

var headingAvailable: Bool

A Boolean value indicating whether the location manager is able to generate heading-related events.

Deprecated

var purpose: String?

An app-provided string that describes the reason for using location services.

Deprecated

var rangedRegions: Set&lt;CLRegion>

The set of regions currently being tracked using ranging.

Deprecated

