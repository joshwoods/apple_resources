

- Force Feedback
-  FFDeviceSendForceFeedbackCommand(\_:\_:) 

Function

# FFDeviceSendForceFeedbackCommand(\_:\_:)

Sends a command to the device’s force feedback system.

Mac Catalyst 13.0+macOS 10.2+

``` source
func FFDeviceSendForceFeedbackCommand(
    _ deviceReference: FFDeviceObjectReference!,
    _ flags: FFCommandFlag
) -> HRESULT
```

## Parameters 

`deviceReference`  

An opaque reference handle to the device object that is be disposed of. This handle is obtained from a previous call to FFCreateDevice.

`flags`  

Single value indicating the desired change in state. The value can be one of the following:

FFSFFC_CONTINUE

Paused playback of all active effects is to be continued. It is an error to send this command when the device is not in a paused state.

FFSFFC_PAUSE

Playback of all active effects is to be paused. This command also stops the clock-on effects so that they continue playing to their full duration when restarted.

While the device is paused, new effects cannot be started, and existing ones cannot be modified. Doing so can cause the subsequent FFSFFC_CONTINUE command to fail to perform properly.

To abandon a pause and stop all effects, use the FFSFFC_STOPALL or FFSFCC_RESET commands.

FFSFFC_RESET

The device’s force feedback system is to be put in its startup state. All effects are removed from the device, are no longer valid, and must be recreated if they are to be used again. The device’s actuators are disabled.

FFSFFC_SETACTUATORSOFF

The device’s force feedback actuators are to be disabled. While the actuators are off, effects continue to play but are ignored by the device. Using the analogy of a sound playback device, they are muted, rather than paused.

FFSFFC_SETACTUATORSON

The device’s force feedback actuators are to be enabled.

FFSFFC_STOPALL

Playback of any active effects is to be stopped. All active effects are reset, but are still being maintained by the device and are still valid. If the device is in a paused state, that state is lost.

This command is equivalent to calling the FFEffect_Stop method for each effect playing.

## Return Value

If the method succeeds, the return value is FF_OK. If the method fails, the return value can be one of the following error values:

## Discussion

FFERR_INVALIDPARAM

FFERR_INTERNAL

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

func FFDeviceGetForceFeedbackState(FFDeviceObjectReference!, UnsafeMutablePointer&lt;FFState>!) -> HRESULT

Retrieves the state of the device’s force feedback system.

func FFDeviceReleaseEffect(FFDeviceObjectReference!, FFEffectObjectReference!) -> HRESULT

Disposes of an API effect object created with FFDeviceCreateEffect.

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

