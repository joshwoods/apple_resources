

- External Accessory
- EAAccessory
-  delegate 

Instance Property

# delegate

The object that acts as the delegate of the accessory.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
unowned(unsafe) var delegate: (any EAAccessoryDelegate)? { get set }
```

## Discussion

The delegate receives notifications about changes to the status of the accessory object. The delegate must adopt the EAAccessoryDelegate protocol.

## See Also

### Responding to Disconnection Events

protocol EAAccessoryDelegate

A protocol that defines an optional method for receiving notifications when the associated accessory object is disconnected.

