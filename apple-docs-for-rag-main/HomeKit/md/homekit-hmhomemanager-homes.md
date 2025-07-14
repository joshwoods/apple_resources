

- HomeKit
- HMHomeManager
-  homes 

Instance Property

# homes

An array of all homes managed by this home manager.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var homes: [HMHome] { get }
```

## Discussion

When you create a new home manager, its homes array is empty by default. You can only be sure that this array is properly initialized with data from the shared HomeKit database after the manager calls its delegate’s homeManagerDidUpdateHomes(_:) method for the first time.

## See Also

### Working with the home layout

class HMHome

The primary unit of living space, typically composed of rooms organized into zones.

