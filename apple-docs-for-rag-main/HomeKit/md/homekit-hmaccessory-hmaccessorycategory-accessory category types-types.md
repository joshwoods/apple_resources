

- HomeKit
- HMAccessory
- HMAccessoryCategory
-  Accessory Category Types 

API Collection

# Accessory Category Types

The accessory category types supported by HomeKit.

## Overview

An HMAccessoryCategory instance’s read-only categoryType property contains one of the values listed below to tell you what the associated accessory does.

Don’t confuse these values with the service types found in Accessory Service Types. Despite the similarities, they describe different things. Accessories are the physical objects that the user installs in the home, like a garage door opener. Accessories belong to one of the categories listed here, like HMAccessoryCategoryTypeGarageDoorOpener.

Accessories have one or more services that perform tasks. The garage door opener accessory has a garage door opener service with service type HMServiceTypeGarageDoorOpener. The same accessory might also have an attached light providing a light bulb service with service type HMServiceTypeLightbulb.

## Topics

### Light

let HMAccessoryCategoryTypeLightbulb: String

A lightbulb accessory.

### Power and switches

let HMAccessoryCategoryTypeOutlet: String

An outlet accessory.

let HMAccessoryCategoryTypeProgrammableSwitch: String

A programmable switch accessory.

let HMAccessoryCategoryTypeSwitch: String

A switch accessory.

### Air quality and smoke detection

let HMAccessoryCategoryTypeFan: String

A fan accessory.

let HMAccessoryCategoryTypeAirPurifier: String

An air purifier accessory.

### Temperature and humidity

let HMAccessoryCategoryTypeThermostat: String

A thermostat accessory.

let HMAccessoryCategoryTypeAirConditioner: String

An air conditioner accessory.

let HMAccessoryCategoryTypeAirDehumidifier: String

A dehumidifier accessory.

let HMAccessoryCategoryTypeAirHeater: String

An air heater accessory.

let HMAccessoryCategoryTypeAirHumidifier: String

A humidifier accessory.

### Windows

let HMAccessoryCategoryTypeWindow: String

A window accessory.

let HMAccessoryCategoryTypeWindowCovering: String

A window covering accessory.

### Locks and openers

let HMAccessoryCategoryTypeDoor: String

A door accessory.

let HMAccessoryCategoryTypeDoorLock: String

A door lock accessory.

let HMAccessoryCategoryTypeGarageDoorOpener: String

A garage door opener accessory.

let HMAccessoryCategoryTypeVideoDoorbell: String

A video doorbell accessory.

### Safety and security

let HMAccessoryCategoryTypeSensor: String

A sensor accessory.

let HMAccessoryCategoryTypeSecuritySystem: String

A security system accessory.

### Cameras

let HMAccessoryCategoryTypeIPCamera: String

A networked camera accessory.

### Water

let HMAccessoryCategoryTypeSprinkler: String

A sprinkler system accessory.

let HMAccessoryCategoryTypeFaucet: String

A faucet accessory.

let HMAccessoryCategoryTypeShowerHead: String

A shower head accessory.

### Network

let HMAccessoryCategoryTypeBridge: String

A bridge accessory.

let HMAccessoryCategoryTypeRangeExtender: String

A range extender accessory.

let HMAccessoryCategoryTypeAirPort: String

An AirPort accessory.

let HMAccessoryCategoryTypeWiFiRouter: String

A WiFi router accessory.

### Audio and sound

let HMAccessoryCategoryTypeAudioReceiver: String

An audio receiver accessory that supports HAP and AirPlay2.

let HMAccessoryCategoryTypeSpeaker: String

A speaker accessory.

### Television

let HMAccessoryCategoryTypeTelevision: String

A television accessory.

let HMAccessoryCategoryTypeTelevisionSetTopBox: String

A television set-top box accessory.

let HMAccessoryCategoryTypeTelevisionStreamingStick: String

A television streaming stick accessory.

### Uncategorized

let HMAccessoryCategoryTypeOther: String

An uncategorized accessory.

## See Also

### Reading the category type

var categoryType: String

The category to which this accessory belongs.

