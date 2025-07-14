

- HomeKit
- HMCharacteristic
-  Characteristic Properties 

API Collection

# Characteristic Properties

The properties that characteristics can have.

## Overview

Check to see if a characteristic’s properties array contains any of these constants to learn something about the corresponding characteristic (HMCharacteristic).

## Topics

### Properties of Characteristics

let HMCharacteristicPropertyReadable: String

The characteristic is readable.

let HMCharacteristicPropertyWritable: String

The characteristic is writable.

let HMCharacteristicPropertyHidden: String

The characteristic should be hidden from the user.

## See Also

### Reading characteristic properties

var properties: [String]

An array of properties that describe the characteristic.

