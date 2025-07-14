

- HomeKit
- HMAccessoryDelegate
-  accessory(\_:service:didUpdateValueFor:) 

Instance Method

# accessory(\_:service:didUpdateValueFor:)

Informs the delegate of a change in value of a characteristic.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
optional func accessory(
    _ accessory: HMAccessory,
    service: HMService,
    didUpdateValueFor characteristic: HMCharacteristic
)
```

## Parameters 

`accessory`  

The accessory.

`service`  

The service with a changed characteristic value.

`characteristic`  

The characteristic whose value changed.

## Mentioned in 

Testing your app with the HomeKit Accessory Simulator

## Discussion

This method is called as a result of a change in value initiated by the accessory. Programmatic changes initiated by the app do not result in this method being called.

## See Also

### Observing accessories

func accessoryDidUpdateName(HMAccessory)

Informs the delegate when the name of the accessory is updated.

func accessoryDidUpdateReachability(HMAccessory)

Informs the delegate when the reachability of the accessory changes.

func accessoryDidUpdateServices(HMAccessory)

Informs the delegate when the services on the accessory have been updated.

func accessory(HMAccessory, didUpdateNameFor: HMService)

Informs the delegate when the name of a service is updated.

func accessory(HMAccessory, didUpdateAssociatedServiceTypeFor: HMService)

Informs the delegate when the associated service type of a service is modified.

func accessory(HMAccessory, didAdd: HMAccessoryProfile)

Informs the delegate when a profile is added to an accessory.

func accessory(HMAccessory, didRemove: HMAccessoryProfile)

Informs the delegate when a profile is removed from an accessory.

func accessory(HMAccessory, didUpdateFirmwareVersion: String)

Informs the delegate when firmwareVersion has been changed for an accessory.

