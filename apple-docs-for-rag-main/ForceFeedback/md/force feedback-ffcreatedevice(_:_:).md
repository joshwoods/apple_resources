

- Force Feedback
-  FFCreateDevice(\_:\_:) 

Function

# FFCreateDevice(\_:\_:)

Creates a new API device object from an OS object in preparation to use the device for force feedback.

Mac Catalyst 13.0+macOS 10.2+

``` source
func FFCreateDevice(
    _ hidDevice: io_service_t,
    _ pDeviceReference: UnsafeMutablePointer!
) -> HRESULT
```

## Parameters 

`hidDevice`  

Pointer to a HID device object.

`pDeviceReference`  

Address of a variable to receive an opaque reference handle to a new device object. This reference can be used in subsequent calls to FFDevice\* functions

## Return Value

If the method succeeds, and the device supports FF, the return value is FF_OK. If the method fails, the return value can be one of the following error values:

## Discussion

FFERR_INVALIDPARAM

FFERR_NOINTERFACE

FFERR_OUTOFMEMORY

FFERR_INTERNAL

## Discussion

When you are finished with the device, FFReleaseDevice must be called on the reference received in this function to dispose of the API device object.

## See Also

### Miscellaneous

func FFDeviceCreateEffect(FFDeviceObjectReference!, CFUUID!, UnsafeMutablePointer&lt;FFEFFECT>!, UnsafeMutablePointer&lt;FFEffectObjectReference?>!) -> HRESULT

Creates and initializes an instance of an effect identified by the effect UUID on the device.

func FFDeviceEscape(FFDeviceObjectReference!, UnsafeMutablePointer&lt;FFEFFESCAPE>!) -> HRESULT

Sends a hardware-specific command to the device.

func FFDeviceGetForceFeedbackCapabilities(FFDeviceObjectReference!, UnsafeMutablePointer&lt;FFCAPABILITIES>!) -> HRESULT

Retrieves the device’s force feedback capabilities.

func FFDeviceGetForceFeedbackProperty(FFDeviceObjectReference!, FFProperty, UnsafeMutableRawPointer!, IOByteCount) -> HRESULT

Gets properties that define the device behavior.

func FFDeviceGetForceFeedbackState(FFDeviceObjectReference!, UnsafeMutablePointer&lt;FFState>!) -> HRESULT

Retrieves the state of the device’s force feedback system.

func FFDeviceReleaseEffect(FFDeviceObjectReference!, FFEffectObjectReference!) -> HRESULT

Disposes of an API effect object created with FFDeviceCreateEffect.

func FFDeviceSendForceFeedbackCommand(FFDeviceObjectReference!, FFCommandFlag) -> HRESULT

Sends a command to the device’s force feedback system.

func FFDeviceSetCooperativeLevel(FFDeviceObjectReference!, UnsafeMutableRawPointer!, FFCooperativeLevelFlag) -> HRESULT

Function is unimplemented in version 1.0 of this API

func FFDeviceSetForceFeedbackProperty(FFDeviceObjectReference!, FFProperty, UnsafeMutableRawPointer!) -> HRESULT

Retrieves the device’s force feedback capabilities.

func FFEffectDownload(FFEffectObjectReference!) -> HRESULT

Places the effect on the device. If the effect is already on the device, the existing effect is updated to match the values set by the FFEffectSetParameters method.

func FFEffectEscape(FFEffectObjectReference!, UnsafeMutablePointer&lt;FFEFFESCAPE>!) -> HRESULT

Sends a hardware-specific command to the driver.

func FFEffectGetEffectStatus(FFEffectObjectReference!, UnsafeMutablePointer&lt;FFEffectStatusFlag>!) -> HRESULT

Sends a hardware-specific command to the driver.

func FFEffectGetParameters(FFEffectObjectReference!, UnsafeMutablePointer&lt;FFEFFECT>!, FFEffectParameterFlag) -> HRESULT

Retrieves information about an effect.

func FFEffectSetParameters(FFEffectObjectReference!, UnsafeMutablePointer&lt;FFEFFECT>!, FFEffectParameterFlag) -> HRESULT

Sets the characteristics of an effect.

func FFEffectStart(FFEffectObjectReference!, UInt32, FFEffectStartFlag) -> HRESULT

Begins playing an effect. If the effect is already playing, it is restarted from the beginning. If the effect has not been downloaded or has been modified since its last download, it is downloaded before being started. This default behavior can be suppressed by passing the FFES_NODOWNLOAD flag.

