

- HomeKit
- HMCharacteristic
- HMCharacteristicMetadata
-  Characteristic Units 

API Collection

# Characteristic Units

Descriptions of the units of a characteristic.

## Overview

Expect to find one of these values in the units property of a characteristic’s metadata.

## Topics

### Parts Per Total

let HMCharacteristicMetadataUnitsPercentage: String

The unit of the characteristic is a percentage.

let HMCharacteristicMetadataUnitsPartsPerMillion: String

The unit of the characters is parts per million.

### Temperature

let HMCharacteristicMetadataUnitsCelsius: String

The unit of the characteristic is celsius.

let HMCharacteristicMetadataUnitsFahrenheit: String

The unit of the characteristic is fahrenheit.

### Time

let HMCharacteristicMetadataUnitsSeconds: String

The unit of the characteristic is seconds.

### Light

let HMCharacteristicMetadataUnitsLux: String

The unit of the characteristic is lux (that is, illuminance).

### Mass

let HMCharacteristicMetadataUnitsMicrogramsPerCubicMeter: String

The unit of the characteristic is micrograms per cubic meter.

### Rotation

let HMCharacteristicMetadataUnitsArcDegree: String

The unit of the characteristic is the degrees of an arc.

## See Also

### Specifying units

var units: String?

The units of the characteristic value.

