

- MatterSupport
- MatterAddDeviceRequest
-  shouldScanNetworks 

Instance Property

# shouldScanNetworks

A flag that indicates whether to receive network scan results.

iOS 16.4+iPadOS 16.4+Mac CatalystmacOS 14.0+visionOS

``` source
var shouldScanNetworks: Bool
```

## Discussion

The app receives the network scan results, or an empty list if no scan occurred. Even if the property is set to `true`, the scan may not occur if the accessory doesn’t support scanning.

## See Also

### Performing the request

func perform() async throws

Launch the user interface to set up a Matter device in the ecosystem.

