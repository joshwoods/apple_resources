

- HomeKit
- HMCharacteristic
-  Characteristic types 

API Collection

# Characteristic types

The characteristic types supported by HomeKit-based accessories.

## Overview

A characteristic’s characteristicType is a string constant—typically containing one of the values listed below—that tells you what the characteristic’s value represents and how to interpret it. Manufacturers can also create custom types, not listed here.

For some characteristic types, HomeKit defines an enumeration of possible values that the corresponding characteristic can take. For example, a characteristic with type HMCharacteristicTypeTemperatureUnits can only have values—corresponding to degrees Fahrenheit or degrees Celsius—from the HMCharacteristicValueTemperatureUnit enumeration.

For other characteristic types, the corresponding value might be a plain number, a string, or Boolean, or a blob of data with encoding specific to that type.

## Topics

### Light

let HMCharacteristicTypeCurrentLightLevel: String

The current light level.

let HMCharacteristicTypeHue: String

The hue of the color used by a light.

let HMCharacteristicTypeBrightness: String

The brightness of a light.

let HMCharacteristicTypeSaturation: String

The saturation of the color used by a light.

let HMCharacteristicTypeColorTemperature: String

The color temperature of a light.

### Power and switches

let HMCharacteristicTypeBatteryLevel: String

The battery level of the accessory.

let HMCharacteristicTypeChargingState: String

The charging state of a battery.

let HMCharacteristicTypeContactState: String

The state of a contact sensor.

let HMCharacteristicTypeOutletInUse: String

The state of an outlet.

let HMCharacteristicTypePowerState: String

The power state of the accessory.

let HMCharacteristicTypeStatusLowBattery: String

A low battery indicator.

let HMCharacteristicTypeOutputState: String

The output state of a programmable switch.

let HMCharacteristicTypeInputEvent: String

The input event of a programmable switch.

let HMCharacteristicTypePowerModeSelection: String

The selected power mode.

### Temperature

let HMCharacteristicTypeCurrentTemperature: String

The current temperature measured by the accessory.

let HMCharacteristicTypeTargetTemperature: String

The target temperature for the accessory to achieve.

let HMCharacteristicTypeTemperatureUnits: String

The units of temperature currently active on the accessory.

let HMCharacteristicTypeTargetHeatingCooling: String

The target heating or cooling mode for a thermostat.

let HMCharacteristicTypeCurrentHeatingCooling: String

The current heating or cooling mode for a thermostat.

let HMCharacteristicTypeTargetHeaterCoolerState: String

The target state for a device that heats or cools, like an oven or a refrigerator.

let HMCharacteristicTypeCurrentHeaterCoolerState: String

The current state for a device that heats or cools, like an oven or a refrigerator.

let HMCharacteristicTypeCoolingThreshold: String

The temperature above which cooling will be active.

let HMCharacteristicTypeHeatingThreshold: String

The temperature below which heating will be active.

### Humidity

let HMCharacteristicTypeCurrentRelativeHumidity: String

The current relative humidity measured by the accessory.

let HMCharacteristicTypeTargetRelativeHumidity: String

The target relative humidity for the accessory to achieve.

let HMCharacteristicTypeCurrentHumidifierDehumidifierState: String

The current state of a humidifier or dehumidifier accessory.

let HMCharacteristicTypeTargetHumidifierDehumidifierState: String

The state that a humidifier or dehumidifier accessory should try to achieve.

let HMCharacteristicTypeHumidifierThreshold: String

The humidity below which a humidifier should begin to work.

let HMCharacteristicTypeDehumidifierThreshold: String

The humidity above which a dehumidifier should begin to work.

### Air quality and smoke detection

let HMCharacteristicTypeAirQuality: String

The air quality.

let HMCharacteristicTypeAirParticulateDensity: String

The density of air-particulate matter.

let HMCharacteristicTypeAirParticulateSize: String

The size of the air-particulate matter.

let HMCharacteristicTypeSmokeDetected: String

A smoke detection indicator.

let HMCharacteristicTypeCarbonDioxideDetected: String

An indicator of abnormally high levels of carbon dioxide.

let HMCharacteristicTypeCarbonDioxideLevel: String

The measured carbon dioxide level.

let HMCharacteristicTypeCarbonDioxidePeakLevel: String

The highest recorded level of carbon dioxide.

let HMCharacteristicTypeCarbonMonoxideDetected: String

An indicator of abnormally high levels of carbon monoxide.

let HMCharacteristicTypeCarbonMonoxideLevel: String

The measured carbon monoxide level.

let HMCharacteristicTypeCarbonMonoxidePeakLevel: String

The highest recorded level of carbon monoxide.

let HMCharacteristicTypeNitrogenDioxideDensity: String

The measured density of nitrogen dioxide.

let HMCharacteristicTypeOzoneDensity: String

The measured density of ozone.

let HMCharacteristicTypePM10Density: String

The measured density of air-particulate matter of size 10 micrograms.

let HMCharacteristicTypePM2_5Density: String

The measured density of air-particulate matter of size 2.5 micrograms.

let HMCharacteristicTypeSulphurDioxideDensity: String

The measured density of sulphur dioxide.

let HMCharacteristicTypeVolatileOrganicCompoundDensity: String

The measured density of volatile organic compounds.

### Fans

let HMCharacteristicTypeCurrentFanState: String

The current state of a fan.

let HMCharacteristicTypeTargetFanState: String

The target state of a fan.

let HMCharacteristicTypeRotationDirection: String

The rotation direction of an accessory like a fan.

let HMCharacteristicTypeRotationSpeed: String

The rotation speed of an accessory like a fan.

let HMCharacteristicTypeSwingMode: String

An indicator of whether a fan swings back and forth during operation.

### Purifiers and filters

let HMCharacteristicTypeCurrentAirPurifierState: String

The current air purifier state.

let HMCharacteristicTypeTargetAirPurifierState: String

The target air purifier state.

let HMCharacteristicTypeFilterLifeLevel: String

The amount of useful life remaining in a filter.

let HMCharacteristicTypeFilterChangeIndication: String

A filter’s change indicator.

let HMCharacteristicTypeFilterResetChangeIndication: String

A reset control for a filter change notification.

### Water

let HMCharacteristicTypeWaterLevel: String

The water level measured by an accessory.

let HMCharacteristicTypeValveType: String

The type of automated valve that controls fluid flow.

let HMCharacteristicTypeLeakDetected: String

A leak detection indicator.

### Doors and windows

let HMCharacteristicTypeCurrentDoorState: String

The current door state.

let HMCharacteristicTypeTargetDoorState: String

The target door state.

let HMCharacteristicTypeCurrentPosition: String

The current position of a door, window, awning, or window covering.

let HMCharacteristicTypeTargetPosition: String

The target position of a door, window, awning, or window covering.

let HMCharacteristicTypePositionState: String

The position of an accessory like a door, window, awning, or window covering.

let HMCharacteristicTypeStatusJammed: String

An indicator of whether an accessory is jammed.

let HMCharacteristicTypeHoldPosition: String

A control for holding the position of an accessory like a door or window.

let HMCharacteristicTypeSlatType: String

The type of slat on an accessory like a window or a fan.

let HMCharacteristicTypeCurrentSlatState: String

The current state of slats on an accessory like a window or a fan.

### Tilting mechanisms

let HMCharacteristicTypeCurrentHorizontalTilt: String

The current tilt angle of a horizontal slat for an accessory like a window or a fan.

let HMCharacteristicTypeTargetHorizontalTilt: String

The target tilt angle of a horizontal slat for an accessory like a window or a fan.

let HMCharacteristicTypeCurrentVerticalTilt: String

The current tilt angle of a vertical slat for an accessory like a window or a fan.

let HMCharacteristicTypeTargetVerticalTilt: String

The target tilt angle of a vertical slat for an accessory like a window or a fan.

let HMCharacteristicTypeCurrentTilt: String

The current tilt angle of a slat for an accessory like a window or a fan.

let HMCharacteristicTypeTargetTilt: String

The target tilt angle of a slat for an accessory like a window or a fan.

### Locks and openers

let HMCharacteristicTypeLockManagementAutoSecureTimeout: String

The automatic timeout for a lockable accessory that supports automatic lockout.

let HMCharacteristicTypeLockManagementControlPoint: String

A control that accepts vendor-specific actions for lock management.

let HMCharacteristicTypeLockMechanismLastKnownAction: String

The last known action of the locking mechanism.

let HMCharacteristicTypeLockPhysicalControls: String

The lock’s physical control state.

let HMCharacteristicTypeMotionDetected: String

An indicator of whether the accessory has detected motion.

let HMCharacteristicTypeCurrentLockMechanismState: String

The current state of the locking mechanism.

let HMCharacteristicTypeTargetLockMechanismState: String

The target state for the locking mechanism.

let HMCharacteristicTypeRemoteKey: String

The accessory remote control key.

### Safety and security

let HMCharacteristicTypeCurrentSecuritySystemState: String

The current security system state.

let HMCharacteristicTypeTargetSecuritySystemState: String

The target security system state.

let HMCharacteristicTypeObstructionDetected: String

An indicator of whether an obstruction is detected, as when something prevents a garage door from closing.

let HMCharacteristicTypeOccupancyDetected: String

An indicator of whether the home is occupied.

let HMCharacteristicTypeSecuritySystemAlarmType: String

The alarm trigger state.

let HMCharacteristicPropertyRequiresAuthorizationData: String

A variable that specifies that the characteristic requires authorization data to write.

### Audio and video

let HMCharacteristicTypeSupportedRTPConfiguration: String

The supported Real-time Transport Protocol (RTP) configuration.

let HMCharacteristicTypeDigitalZoom: String

The digital zoom of a video Real-time Transport Protocol (RTP) service.

let HMCharacteristicTypeOpticalZoom: String

The optical zoom setting of the camera sourcing a video Real-time Transport Protocol (RTP) service.

let HMCharacteristicTypeImageMirroring: String

An indicator of whether the image should be flipped about the vertical axis.

let HMCharacteristicTypeImageRotation: String

The angle of rotation for an image.

let HMCharacteristicTypeNightVision: String

An indicator of whether night vision is enabled on a video Real-time Transport Protocol (RTP) service.

let HMCharacteristicTypeStreamingStatus: String

A description of the status of the Real-time Transport Protocol (RTP) stream management service.

let HMCharacteristicTypeSupportedVideoStreamConfiguration: String

The video stream’s configuration.

let HMCharacteristicTypeSupportedAudioStreamConfiguration: String

The audio stream’s configuration.

let HMCharacteristicTypeSelectedStreamConfiguration: String

The selected stream’s configuration.

let HMCharacteristicTypeSetupStreamEndpoint: String

The stream’s endpoint configuration.

let HMCharacteristicTypeAudioFeedback: String

An indicator of whether audio feedback, like a beep or other external sound mechanism, is enabled.

let HMCharacteristicTypeVolume: String

The input or output volume of an audio device.

let HMCharacteristicTypeMute: String

A control for muting audio.

let HMCharacteristicTypeVolumeSelector: String

The mechanism to increment or decrement the volume by the default step value.

let HMCharacteristicTypeVolumeControlType: String

The volume control capabilities of an accessory.

let HMCharacteristicTypeClosedCaptions: String

An indictator of whether closed captions are enabled or disabled.

let HMCharacteristicTypePictureMode: String

The selected picture mode.

### General state

let HMCharacteristicTypeActive: String

The current status of an accessory.

let HMCharacteristicTypeStatusTampered: String

An indicator of whether an accessory has been tampered with.

let HMCharacteristicTypeStatusFault: String

An indicator of whether the accessory has experienced a fault.

let HMCharacteristicTypeStatusActive: String

An indicator of whether the service is working.

let HMCharacteristicTypeInUse: String

The current usage state of an accessory.

let HMCharacteristicTypeIsConfigured: String

The configuration state of an accessory.

let HMCharacteristicTypeRemainingDuration: String

The number of seconds remaining for the activity being carried out by the accessory.

let HMCharacteristicTypeSetDuration: String

The duration of the activity being carried out by the accessory.

let HMCharacteristicTypeProgramMode: String

The current mode of the accessory’s scheduled programs.

let HMCharacteristicTypeWiFiSatelliteStatus: String

The network status of the WiFi satellite accessory.

let HMCharacteristicTypeWANStatusList: String

The WAN status list of an accessory.

let HMCharacteristicTypeTargetMediaState: String

The target media state.

let HMCharacteristicTypeRouterStatus: String

The current status of the router.

let HMCharacteristicTypeCurrentMediaState: String

The current state of the media.

let HMCharacteristicTypeCurrentVisibilityState: String

The current visibility state for a service.

let HMCharacteristicTypeTargetVisibilityState: String

The target visibility state for a service.

let HMCharacteristicPropertySupportsEventNotification: String

The characteristic supports event notifications.

### Accessory identification

let HMCharacteristicTypeName: String

The name of the accessory.

let HMCharacteristicTypeIdentify: String

A control you can use to ask the accessory to identify itself.

let HMCharacteristicTypeVersion: String

The version of the accessory.

let HMCharacteristicTypeLogs: String

Log data for the accessory.

let HMCharacteristicTypeAdminOnlyAccess: String

An indicator of whether the accessory accepts only administrator access.

let HMCharacteristicTypeHardwareVersion: String

The hardware version of the accessory.

let HMCharacteristicTypeSoftwareVersion: String

The software version of the accessory.

let HMCharacteristicTypeLabelIndex: String

The index of the label for the service on an accessory with multiple instances of the same service.

let HMCharacteristicTypeLabelNamespace: String

The naming schema used to label the services on an accessory with multiple services of the same type.

let HMCharacteristicTypeActiveIdentifier: String

An index that maps to the current active Input Source service.

let HMCharacteristicTypeIdentifier: String

The identifier for an accessory.

let HMCharacteristicTypeInputDeviceType: String

The accessory input device type.

let HMCharacteristicTypeInputSourceType: String

The accessory input source type.

let HMCharacteristicTypeConfiguredName: String

A `UTF‑8` encoded user visible name on an accessory.

### Deprecated characteristic types

let HMCharacteristicTypeManufacturer: String

The manufacturer of the accessory.

Deprecated

let HMCharacteristicTypeModel: String

The model of the accessory.

Deprecated

let HMCharacteristicTypeFirmwareVersion: String

The firmware version of the accessory.

Deprecated

let HMCharacteristicTypeSerialNumber: String

The serial number of the accessory.

Deprecated

## See Also

### Determining what a characteristic controls

var characteristicType: String

The type of the characteristic.

