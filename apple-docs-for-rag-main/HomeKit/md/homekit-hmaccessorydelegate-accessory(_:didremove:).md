

- HomeKit
- HMAccessoryDelegate
-  accessory(\_:didRemove:) 

Instance Method

# accessory(\_:didRemove:)

Informs the delegate when a profile is removed from an accessory.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional func accessory(
    _ accessory: HMAccessory,
    didRemove profile: HMAccessoryProfile
)
```

## Parameters 

`accessory`  

The accessory from which the profile is removed.

`profile`  

The removed profile.

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

func accessory(HMAccessory, service: HMService, didUpdateValueFor: HMCharacteristic)

Informs the delegate of a change in value of a characteristic.

func accessory(HMAccessory, didUpdateAssociatedServiceTypeFor: HMService)

Informs the delegate when the associated service type of a service is modified.

func accessory(HMAccessory, didAdd: HMAccessoryProfile)

Informs the delegate when a profile is added to an accessory.

func accessory(HMAccessory, didUpdateFirmwareVersion: String)

Informs the delegate when firmwareVersion has been changed for an accessory.

