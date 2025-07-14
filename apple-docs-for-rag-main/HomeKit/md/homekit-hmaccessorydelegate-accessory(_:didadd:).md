

- HomeKit
- HMAccessoryDelegate
-  accessory(\_:didAdd:) 

Instance Method

# accessory(\_:didAdd:)

Informs the delegate when a profile is added to an accessory.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
optional func accessory(
    _ accessory: HMAccessory,
    didAdd profile: HMAccessoryProfile
)
```

## Parameters 

`accessory`  

The accessory that has received a new profile.

`profile`  

The newly added profile.

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

func accessory(HMAccessory, didRemove: HMAccessoryProfile)

Informs the delegate when a profile is removed from an accessory.

func accessory(HMAccessory, didUpdateFirmwareVersion: String)

Informs the delegate when firmwareVersion has been changed for an accessory.

