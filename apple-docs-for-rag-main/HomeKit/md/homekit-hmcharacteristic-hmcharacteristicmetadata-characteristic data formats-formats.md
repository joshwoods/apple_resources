

- HomeKit
- HMCharacteristic
- HMCharacteristicMetadata
-  Characteristic Data Formats 

API Collection

# Characteristic Data Formats

Constants for identifying the data format of characteristic values.

## Overview

Expect to find one of these values in the format property of a characteristic’s metadata.

## Topics

### Booleans

let HMCharacteristicMetadataFormatBool: String

Indicates that the characteristic has Boolean values.

### Strings

let HMCharacteristicMetadataFormatString: String

Indicates that the characteristic has string values.

### Signed Values

let HMCharacteristicMetadataFormatInt: String

Indicates that the characteristic has `int` values.

let HMCharacteristicMetadataFormatFloat: String

Indicates that the characteristic has `float` values.

### Unsigned Integers

let HMCharacteristicMetadataFormatUInt8: String

Indicates that the characteristic has unsigned 8-bit integer values.

let HMCharacteristicMetadataFormatUInt16: String

Indicates that the characteristic has unsigned 16-bit integer values.

let HMCharacteristicMetadataFormatUInt32: String

Indicates that the characteristic has unsigned 32-bit integer values.

let HMCharacteristicMetadataFormatUInt64: String

Indicates that the characteristic has unsigned 64-bit integer values.

### Data

let HMCharacteristicMetadataFormatData: String

Indicates that the characteristic has data blob values.

let HMCharacteristicMetadataFormatTLV8: String

Indicates that the characteristic has TLV8 values.

### Collections

let HMCharacteristicMetadataFormatArray: String

Indicates that the characteristic has array values.

let HMCharacteristicMetadataFormatDictionary: String

Indicates that the characteristic has dictionary values.

## See Also

### Formatting the value

var format: String?

The format of the values for the characteristic.

