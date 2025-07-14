

- HomeKit
- HMHomeManager
-  delegate 

Instance Property

# delegate

A delegate that receives updates on the collection of homes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
weak var delegate: (any HMHomeManagerDelegate)? { get set }
```

## See Also

### Keeping track of connected homes

protocol HMHomeManagerDelegate

An interface the home manager uses to communicate changes to the state of the home network.

