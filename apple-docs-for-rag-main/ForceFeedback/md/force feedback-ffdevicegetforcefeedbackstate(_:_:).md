

- Force Feedback
-  FFDeviceGetForceFeedbackState(\_:\_:) 

Function

# FFDeviceGetForceFeedbackState(\_:\_:)

Retrieves the state of the device’s force feedback system.

Mac Catalyst 13.0+macOS 10.2+

``` source
func FFDeviceGetForceFeedbackState(
    _ deviceReference: FFDeviceObjectReference!,
    _ pFFState: UnsafeMutablePointer!
) -> HRESULT
```

## Parameters 

`deviceReference`  

An opaque reference handle to a device object. This is obtained from a previous call to FFCreateDevice.

`pFFState`  

Location for flags that describe the current state of the device’s force feedback system. The value is a combination of the following constants:

FFGFFS_ACTUATORSOFF

The device’s force feedback actuators are disabled.

FFGFFS_ACTUATORSON

The device’s force feedback actuators are enabled.

FFGFFS_DEVICELOST

The device suffered an unexpected failure and is in an indeterminate state. It must be reset either by unacquiring and reacquiring the device, or by sending a FFSFFC_RESET command.

FFGFFS_EMPTY

The device has no downloaded effects.

FFGFFS_PAUSED

Playback of all active effects has been paused.

FFGFFS_POWEROFF

The force feedback system is not currently available. If the device cannot report the power state, neither FFGFFS_POWERON nor FFGFFS_POWEROFF is returned.

FFGFFS_POWERON

Power to the force feedback system is currently available. If the device cannot report the power state, neither FFGFFS_POWERON nor FFGFFS_POWEROFF is returned.

FFGFFS_SAFETYSWITCHOFF

The safety switch is currently off; that is, the device cannot operate. If the device cannot report the state of the safety switch, neither FFGFFS_SAFETYSWITCHON nor FFGFFS_SAFETYSWITCHOFF is returned.

FFGFFS_SAFETYSWITCHON

The safety switch is currently on; that is, the device can operate. If the device cannot report the state of the safety switch, neither FFGFFS_SAFETYSWITCHON nor FFGFFS_SAFETYSWITCHOFF is returned.

FFGFFS_STOPPED

No effects are playing, and the device is not paused.

FFGFFS_USERFFSWITCHOFF

The user force feedback switch is currently off; that is, the device cannot operate. If the device cannot report the state of the user force feedback switch, neither FFGFFS_USERFFSWITCHON nor FFGFFS_USERFFSWITCHOFF is returned.

FFGFFS_USERFFSWITCHON

The user force feedback switch is currently on; that is, the device can operate. If the device cannot report the state of the user force feedback switch, neither FFGFFS_USERFFSWITCHON nor FFGFFS_USERFFSWITCHOFF is returned.

Future versions can define additional flags. Applications should ignore any flags that are not currently defined.

## Return Value

If the method succeeds, the return value is FF_OK. If the method fails, the return value can be one of the following error values:

## Discussion

FFERR_INVALIDPARAM

## See Also

### Miscellaneous

func FFCreateDevice(io_service_t, UnsafeMutablePointer&lt;FFDeviceObjectReference?>!) -> HRESULT

Creates a new API device object from an OS object in preparation to use the device for force feedback.

func FFDeviceCreateEffect(FFDeviceObjectReference!, CFUUID!, UnsafeMutablePointer&lt;FFEFFECT>!, UnsafeMutablePointer&lt;FFEffectObjectReference?>!) -> HRESULT

Creates and initializes an instance of an effect identified by the effect UUID on the device.

func FFDeviceEscape(FFDeviceObjectReference!, UnsafeMutablePointer&lt;FFEFFESCAPE>!) -> HRESULT

Sends a hardware-specific command to the device.

func FFDeviceGetForceFeedbackCapabilities(FFDeviceObjectReference!, UnsafeMutablePointer&lt;FFCAPABILITIES>!) -> HRESULT

Retrieves the device’s force feedback capabilities.

func FFDeviceGetForceFeedbackProperty(FFDeviceObjectReference!, FFProperty, UnsafeMutableRawPointer!, IOByteCount) -> HRESULT

Gets properties that define the device behavior.

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

