

- HomeKit
-  HMCharacteristicMetadata 

Class

# HMCharacteristicMetadata

Metadata that describes a characteristic’s value and that may be useful for presentation purposes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
class HMCharacteristicMetadata
```

## Overview

Querying a characteristic’s metadata enables you to build a user interface that reflects the underlying units, minima, and maxima, and other aspects of the characteristic value.

## Topics

### Describing a characteristic

var manufacturerDescription: String?

A description of the characteristic provided by the accessory manufacturer.

### Bounding the value

var validValues: [NSNumber]?

The subset of valid values supported by the characteristic when the format is of type unsigned integer.

var minimumValue: NSNumber?

The minimum value for the characteristic.

var maximumValue: NSNumber?

The maximum value for the characteristic.

var stepValue: NSNumber?

The minimum interval between values for the characteristic.

var maxLength: NSNumber?

The maximum number of UTF-8 characters allowed in a characteristic that uses a string format.

### Formatting the value

var format: String?

The format of the values for the characteristic.

Characteristic Data Formats

Constants for identifying the data format of characteristic values.

### Specifying units

var units: String?

The units of the characteristic value.

Characteristic Units

Descriptions of the units of a characteristic.

### Initializers

init()

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Managing characteristic presentation

var metadata: HMCharacteristicMetadata?

Metadata about the units and other properties of the characteristic.

