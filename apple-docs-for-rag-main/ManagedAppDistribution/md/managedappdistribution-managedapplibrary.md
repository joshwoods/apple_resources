

- ManagedAppDistribution
-  ManagedAppLibrary 

Class

# ManagedAppLibrary

A representation of a library of managed apps.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
final class ManagedAppLibrary
```

## Mentioned in 

Fetching and displaying managed apps

## Topics

### Obtaining library information

var availableApps: ManagedAppLibrary.ManagedApps

The current managed apps available to this device.

struct ManagedApps

An array of managed apps that updates as apps become available or unavailable.

static let currentDistributor: ManagedAppLibrary

The library provider for managed apps on this device.

## Relationships

### Conforms To

- Sendable

## See Also

### Essentials

Fetching and displaying managed apps

Provide a consistent app presentation when displaying managed apps.

struct ManagedApp

A representation of a managed app.

