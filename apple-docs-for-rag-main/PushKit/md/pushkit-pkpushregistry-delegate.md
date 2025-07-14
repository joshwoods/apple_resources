

- PushKit
- PKPushRegistry
-  delegate 

Instance Property

# delegate

The delegate object that receives notifications coming from the push registry object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
weak var delegate: (any PKPushRegistryDelegate)? { get set }
```

## Discussion

You must assign a valid object to this property before modifying the desiredPushTypes property. A valid delegate object is required to receive push tokens and payload data from incoming pushes.

For more information about the methods of the `PKPushRegistryDelegate` protocol, see PKPushRegistryDelegate.

## See Also

### Receiving the Notification Data

protocol PKPushRegistryDelegate

The methods that you use to handle incoming PushKit notifications and registration events.

