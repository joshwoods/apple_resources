

- Screen Time
-  STScreenTimeConfigurationObserver 

Class

# STScreenTimeConfigurationObserver

The object you use to observe changes to the current configuration.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+

``` source
class STScreenTimeConfigurationObserver
```

## Overview

Use this class to start and stop observing the current configuration. For example, you can opt to disable private browsing in your web browser’s view controller when enforcesChildRestrictions is `true`.

## Topics

### Initializers

init(updateQueue: dispatch_queue_t)

Creates a configuration observer that reports updates on the queue you specify.

### Instance properties

var configuration: STScreenTimeConfiguration?

The configuration being observed.

### Instance methods

func startObserving()

Starts observing changes to the current configuration.

func stopObserving()

Stops observing changes to the current configuration.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Configuration queries

class STScreenTimeConfiguration

The configuration for this device.

