

- ManagedAppDistribution
- ManagedAppLibrary
-  availableApps 

Instance Property

# availableApps

The current managed apps available to this device.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
final var availableApps: ManagedAppLibrary.ManagedApps { get }
```

## Discussion

The current managed apps are of type `Result`. Use an asynchronous `for` loop to update your views when the current managed apps change. If the device can’t retrieve the metadata for the apps, fetching the list of managed apps fails with `ManagedAppDistributionError.networkError`. An example of this failure is if the device is offline.

Note

The async sequence returns an error and the sequence ends when running as an iOS app on macOS.

## See Also

### Obtaining library information

struct ManagedApps

An array of managed apps that updates as apps become available or unavailable.

static let currentDistributor: ManagedAppLibrary

The library provider for managed apps on this device.

