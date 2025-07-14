

- Core Location
- CLLocationManager
-  headingAvailable Deprecated

Instance Property

# headingAvailable

A Boolean value indicating whether the location manager is able to generate heading-related events.

macOS 10.15–10.15DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var headingAvailable: Bool { get }
```

Deprecated

Use the headingAvailable() class method instead.

## Discussion

Heading data may not be available on all iOS-based devices. You should check the value of this property before asking the location manager to deliver heading-related events.

