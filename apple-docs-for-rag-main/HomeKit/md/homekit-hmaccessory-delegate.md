

- HomeKit
- HMAccessory
-  delegate 

Instance Property

# delegate

A delegate that receives updates on the state of the accessory.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
weak var delegate: (any HMAccessoryDelegate)? { get set }
```

## See Also

### Tracking changes to an accessory

protocol HMAccessoryDelegate

A set of methods that defines the communication method for state updates from accessories to their delegates.

