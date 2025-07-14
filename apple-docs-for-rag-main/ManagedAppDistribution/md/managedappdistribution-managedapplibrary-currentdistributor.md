

- ManagedAppDistribution
- ManagedAppLibrary
-  currentDistributor 

Type Property

# currentDistributor

The library provider for managed apps on this device.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
static let currentDistributor: ManagedAppLibrary
```

## Discussion

This is a singleton object.

## See Also

### Obtaining library information

var availableApps: ManagedAppLibrary.ManagedApps

The current managed apps available to this device.

struct ManagedApps

An array of managed apps that updates as apps become available or unavailable.

