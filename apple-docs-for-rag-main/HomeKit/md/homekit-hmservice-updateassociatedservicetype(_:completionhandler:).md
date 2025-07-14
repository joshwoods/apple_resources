

- HomeKit
- HMService
-  updateAssociatedServiceType(\_:completionHandler:) 

Instance Method

# updateAssociatedServiceType(\_:completionHandler:)

Associates the service type of the plugged-in device with a switch or an outlet service.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+visionOS 1.0+

``` source
func updateAssociatedServiceType(
    _ serviceType: String?,
    completionHandler completion: @escaping ((any Error)?) -> Void
)
```

``` source
func updateAssociatedServiceType(_ serviceType: String?) async throws
```

## Parameters 

`serviceType`  

The service type of the device that is hooked up to the switch or outlet.

`completion`  

The block executed after the request is processed.

error  
`nil` on success; otherwise, error object indicating the reason for failure.

## Discussion

This method is only valid for services of type HMServiceTypeOutlet or HMServiceTypeSwitch. See associatedServiceType for details of associated service types.

## See Also

### Associating a secondary service

var associatedServiceType: String?

The type of the service associated with an outlet or a switch.

