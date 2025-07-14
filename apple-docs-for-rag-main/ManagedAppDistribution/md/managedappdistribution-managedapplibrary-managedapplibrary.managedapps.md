

- ManagedAppDistribution
- ManagedAppLibrary
-  ManagedAppLibrary.ManagedApps 

Structure

# ManagedAppLibrary.ManagedApps

An array of managed apps that updates as apps become available or unavailable.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
struct ManagedApps
```

## Topics

### Obtaining managed apps

struct AsyncIterator

The iterator for managed apps.

typealias Element

The type of element this asynchronous sequence produces.

func makeAsyncIterator() -> ManagedAppLibrary.ManagedApps.AsyncIterator

Creates the asynchronous iterator that produces results from this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Obtaining library information

var availableApps: ManagedAppLibrary.ManagedApps

The current managed apps available to this device.

static let currentDistributor: ManagedAppLibrary

The library provider for managed apps on this device.

