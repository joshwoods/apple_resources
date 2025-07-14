

- HomeKit
- HMService
-  associatedServiceType 

Instance Property

# associatedServiceType

The type of the service associated with an outlet or a switch.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
var associatedServiceType: String? { get }
```

## Discussion

Because different things can be plugged into outlets or controlled by switches, there is a tight association between a switch or outlet service and another service that it controls—for example, a lamp plugged into an outlet associates a lightbulb service with the outlet, even if the lamp itself is not a supported HomeKit accessory.

The associated service can be any service defined by the HomeKit Accessory Profile that supports HMCharacteristicTypePowerState, other than HMServiceTypeOutlet or HMServiceTypeSwitch.

See Accessory Service Types for a list of service types.

## See Also

### Associating a secondary service

func updateAssociatedServiceType(String?, completionHandler: ((any Error)?) -> Void)

Associates the service type of the plugged-in device with a switch or an outlet service.

