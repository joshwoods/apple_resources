

- Force Feedback
-  FFDeviceCreateEffect(\_:\_:\_:\_:) 

Function

# FFDeviceCreateEffect(\_:\_:\_:\_:)

Creates and initializes an instance of an effect identified by the effect UUID on the device.

Mac Catalyst 13.0+macOS 10.2+

``` source
func FFDeviceCreateEffect(
    _ deviceReference: FFDeviceObjectReference!,
    _ uuidRef: CFUUID!,
    _ pEffectDefinition: UnsafeMutablePointer!,
    _ pEffectReference: UnsafeMutablePointer!
) -> HRESULT
```

## Parameters 

`deviceReference`  

An opaque reference handle to a device object. This is obtained from a previous call to FFCreateDevice.

`uuidRef`  

Reference to the UUID identifying the effect to be created. Only predefined effect UUIDs are accepted. The following standard effect UUIDs are defined:

kFFEffectType_ConstantForce_ID

kFFEffectType_RampForce_ID

kFFEffectType_Square_ID

kFFEffectType_Sine_ID

kFFEffectType_Triangle_ID

kFFEffectType_SawtoothUp_ID

kFFEffectType_SawtoothDown_ID

kFFEffectType_Spring_ID

kFFEffectType_Damper_ID

kFFEffectType_Inertia_ID

kFFEffectType_Friction_ID

kFFEffectType_CustomForce_ID

`pEffectDefinition`  

Pointer to FFEFFECT structure that provides parameters for the created effect. This parameter is optional. If it is NULL, the effect object is created without parameters. The application must then call the FFEffectSetParameters function to set the parameters of the effect before it can download the effect.

`pEffectReference`  

Address of a variable to receive an opaque reference handle to a new effect object. This reference can be used in subsequent calls to FFEffect\* functions.

## Return Value

If the method succeeds, the return value is FF_OK. If the method fails, the return value can be one of the following error values:

## Discussion

FFERR_INVALIDPARAM

FFERR_UNSUPPORTEDAXIS

FFERR_OUTOFMEMORY

FFERR_DEVICEPAUSED

FFERR_DEVICEFULL

FFERR_INVALIDDOWNLOADID

FFERR_INTERNAL

FFERR_EFFECTTYPEMISMATCH

## Discussion

When you are finished with the effect, FFReleaseEffect must be called on the reference received in this function to dispose of the API effect object.

## See Also

### Miscellaneous

func FFCreateDevice(io_service_t, UnsafeMutablePointer&lt;FFDeviceObjectReference?>!) -> HRESULT

Creates a new API device object from an OS object in preparation to use the device for force feedback.

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

