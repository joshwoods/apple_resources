

- HomeKit
- HMAccessoryDelegate
-  accessoryDidUpdateReachability(\_:) 

Instance Method

# accessoryDidUpdateReachability(\_:)

Informs the delegate when the reachability of the accessory changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
optional func accessoryDidUpdateReachability(_ accessory: HMAccessory)
```

## Parameters 

`accessory`  

The accessory whose reachability has changed.

## Discussion

Accessories expose their reachability via the isReachable property.

## See Also

### Observing accessories

func accessoryDidUpdateName(HMAccessory)

Informs the delegate when the name of the accessory is updated.

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

func accessory(HMAccessory, didRemove: HMAccessoryProfile)

Informs the delegate when a profile is removed from an accessory.

func accessory(HMAccessory, didUpdateFirmwareVersion: String)

Informs the delegate when firmwareVersion has been changed for an accessory.

