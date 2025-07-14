

- MatterSupport
- MatterAddDeviceExtensionRequestHandler
-  commissionDevice(in:onboardingPayload:commissioningID:) 

Instance Method

# commissionDevice(in:onboardingPayload:commissioningID:)

Commissions the device with the onboarding payload.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 14.0+visionOS

``` source
func commissionDevice(
    in home: MatterAddDeviceRequest.Home?,
    onboardingPayload: String,
    commissioningID: UUID
) async throws
```

## Parameters 

`home`  

The selected home for the device.

`onboardingPayload`  

The onboarding payload, as defined by Matter specification, that you need to use to commission the device.

`commissioningID`  

A generated identifier you use with other MatterSupport methods.

