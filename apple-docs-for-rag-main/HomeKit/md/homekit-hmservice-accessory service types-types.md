

- HomeKit
- HMService
-  Accessory Service Types 

API Collection

# Accessory Service Types

The service types supported by HomeKit.

## Overview

An HMService instance’s read-only serviceType property contains one of the values listed below to tell you what the service does.

Don’t confuse these values with the accessory categories found in Accessory Category Types. Despite the similarities, they describe different things. Accessories are the physical objects that the user installs in the home, like a garage door opener. Accessories belong to a particular category, like HMAccessoryCategoryTypeGarageDoorOpener.

Accessories have one or more services that perform tasks. The garage door opener accessory has a garage door opener service with service type HMServiceTypeGarageDoorOpener, given below. The same accessory might also have an attached light providing a light bulb service with service type HMServiceTypeLightbulb, also given below.

## Topics

### Light

let HMServiceTypeLightbulb: String

A light bulb service.

let HMServiceTypeLightSensor: String

A light sensor service.

### Power and Switches

let HMServiceTypeSwitch: String

A switch service.

let HMServiceTypeBattery: String

A battery service.

let HMServiceTypeOutlet: String

An outlet service.

let HMServiceTypeStatefulProgrammableSwitch: String

A stateful programmable switch service.

let HMServiceTypeStatelessProgrammableSwitch: String

A stateless programmable switch service.

### Air Quality and Smoke Detection

let HMServiceTypeAirPurifier: String

An air purifier service.

let HMServiceTypeAirQualitySensor: String

An air quality sensor service.

let HMServiceTypeCarbonDioxideSensor: String

A carbon dioxide sensor service.

let HMServiceTypeCarbonMonoxideSensor: String

A carbon monoxide sensor service.

let HMServiceTypeSmokeSensor: String

A smoke sensor service.

### Temperature and Humidity

let HMServiceTypeHeaterCooler: String

A heater or cooler service.

let HMServiceTypeTemperatureSensor: String

A temperature sensor service.

let HMServiceTypeThermostat: String

A thermostat service.

let HMServiceTypeFan: String

A fan service.

let HMServiceTypeFilterMaintenance: String

A filter maintenance service.

let HMServiceTypeHumidifierDehumidifier: String

A humidifier or dehumidifier service.

let HMServiceTypeHumiditySensor: String

A humidity sensor service.

let HMServiceTypeVentilationFan: String

A ventilation fan service.

### Windows

let HMServiceTypeWindow: String

A window service.

let HMServiceTypeWindowCovering: String

A window covering service.

let HMServiceTypeSlats: String

A slats service.

### Water

let HMServiceTypeFaucet: String

A faucet service.

let HMServiceTypeValve: String

A valve service.

let HMServiceTypeIrrigationSystem: String

An irrigation system service.

let HMServiceTypeLeakSensor: String

A leak sensor service.

### Locks and Openers

let HMServiceTypeDoor: String

A door service.

let HMServiceTypeDoorbell: String

A doorbell service.

let HMServiceTypeGarageDoorOpener: String

A garage door opener service.

let HMServiceTypeLockManagement: String

A lock management service.

let HMServiceTypeLockMechanism: String

A lock mechanism service.

### Safety and Security

let HMServiceTypeMotionSensor: String

A motion sensor service.

let HMServiceTypeOccupancySensor: String

An occupancy sensor service.

let HMServiceTypeSecuritySystem: String

A security system service.

let HMServiceTypeContactSensor: String

A contact sensor service.

### Video and Audio

let HMServiceTypeCameraControl: String

A camera control service.

let HMServiceTypeCameraRTPStreamManagement: String

A stream management service.

let HMServiceTypeMicrophone: String

A microphone service.

let HMServiceTypeSpeaker: String

An audio speaker service.

let HMServiceTypeInputSource: String

An accessory input source service.

let HMServiceTypeTelevision: String

A television service.

### Network

let HMServiceTypeWiFiRouter: String

A WiFi router service.

let HMServiceTypeWiFiSatellite: String

A Satellite WiFi router service.

### Information

let HMServiceTypeLabel: String

A label namespace service used when an accessory supports multiple services of the same type.

let HMServiceTypeAccessoryInformation: String

An accessory information service.

## See Also

### Getting the service type

var serviceType: String

The type of the service.

var localizedDescription: String

The localized description of the service.

