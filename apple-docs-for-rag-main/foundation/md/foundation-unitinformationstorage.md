

- Foundation
-  UnitInformationStorage 

Class

# UnitInformationStorage

A unit of measure for quantities of information.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class UnitInformationStorage
```

## Overview

Use instances of UnitInformationStorage to represent quantities of information using the NSMeasurement class. The base unit of measure for information is the bit, with a nibble representing four bits and a byte representing eight bits.

Larger units of information expand on bits and bytes by orders of magnitude in both decimal and binary forms.

### Information Transfer

Units of bits commonly represent the amount of transferred information.

| Decimal Bits | Coefficient | Binary Bits | Coefficient |
|----|----|----|----|
| kilobits | `1000` | kibibits | `1024` |
| megabits | `1000e2` | mebibits | `1024e2` |
| gigabits | `1000e3` | gibibits | `1024e3` |
| terabits | `1000e4` | tebibits | `1024e4` |
| petabits | `1000e5` | pebibits | `1024e5` |
| exabits | `1000e6` | exbibits | `1024e6` |
| zettabits | `1000e7` | zebibits | `1024e7` |
| yottabits | `1000e8` | yobibits | `1024e8` |

### Information Storage

Units of bytes commonly represent the amount of stored information.

| Decimal Bytes | Coefficient | Binary Bytes | Coefficient |
|----|----|----|----|
| kilobytes | `1000` | kibibytes | `1024` |
| megabytes | `1000e2` | mebibytes | `1024e2` |
| gigabytes | `1000e3` | gibibytes | `1024e3` |
| terabytes | `1000e4` | tebibytes | `1024e4` |
| petabytes | `1000e5` | pebibytes | `1024e5` |
| exabytes | `1000e6` | exbibytes | `1024e6` |
| zettabytes | `1000e7` | zebibytes | `1024e7` |
| yottabytes | `1000e8` | yobibytes | `1024e8` |

## Topics

### Accessing Predefined Common Units

class var bits: UnitInformationStorage

The bits unit of information.

class var nibbles: UnitInformationStorage

The nibbles unit of information.

class var bytes: UnitInformationStorage

The bytes unit of information.

### Accessing Predefined Binary Units

class var kibibits: UnitInformationStorage

The kibibits unit of information.

class var kibibytes: UnitInformationStorage

The kibibytes unit of information.

class var mebibits: UnitInformationStorage

The mebibits unit of information.

class var mebibytes: UnitInformationStorage

The mebibytes unit of information.

class var gibibits: UnitInformationStorage

The gibibits unit of information.

class var gibibytes: UnitInformationStorage

The gibibytes unit of information.

class var tebibits: UnitInformationStorage

The tebibits unit of information.

class var tebibytes: UnitInformationStorage

The tebibytes unit of information.

class var pebibits: UnitInformationStorage

The pebibits unit of information.

class var pebibytes: UnitInformationStorage

The pebibytes unit of information.

class var exbibits: UnitInformationStorage

The exbibits unit of information.

class var exbibytes: UnitInformationStorage

The exbibytes unit of information.

class var zebibits: UnitInformationStorage

The zebibits unit of information.

class var zebibytes: UnitInformationStorage

The zebibytes unit of information.

class var yobibits: UnitInformationStorage

The yobibits unit of information.

class var yobibytes: UnitInformationStorage

The yobibytes unit of information.

### Accessing Predefined Decimal Units

class var kilobits: UnitInformationStorage

The kilobits unit of information.

class var kilobytes: UnitInformationStorage

The kilobytes unit of information.

class var megabits: UnitInformationStorage

The megabits unit of information.

class var megabytes: UnitInformationStorage

The megabytes unit of information.

class var gigabits: UnitInformationStorage

The gigabits unit of information.

class var gigabytes: UnitInformationStorage

The gigabytes unit of information.

class var terabits: UnitInformationStorage

The terabits unit of information.

class var terabytes: UnitInformationStorage

The terrabytes unit of information.

class var petabits: UnitInformationStorage

The petabits unit of information.

class var petabytes: UnitInformationStorage

The petabytes unit of information.

class var exabits: UnitInformationStorage

The exabits unit of information.

class var exabytes: UnitInformationStorage

The exabytes unit of information.

class var zettabits: UnitInformationStorage

The zettabits unit of information.

class var zettabytes: UnitInformationStorage

The zettabytes unit of information.

class var yottabits: UnitInformationStorage

The yottabits unit of information.

class var yottabytes: UnitInformationStorage

The yottabytes unit of information.

## Relationships

### Inherits From

- Dimension

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

