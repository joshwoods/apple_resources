

- Core Services
- Apple Events
-  Numeric Descriptor Type Constants 

# Numeric Descriptor Type Constants

Specify types for numeric descriptors.

## Overview

The constants described here specify the data type for a descriptor and show the kind of numeric data stored in a descriptor with that type. These constants are preferred over their older equivalents described in `typeSMInt`.

Descriptors are the building blocks used by the Apple Event Manager to construct Apple event attributes and parameters. A descriptor is a data structure of type AEDesc, which consists of data storage and a descriptor type that identifies the type of the data. A descriptor type is defined by the data type DescType.

AppleScript defines descriptor type constants for a wide variety of common data types. For additional types, see Descriptor Type Constants and Other Descriptor Type Constants. For a complete listing, including data types such as units of length, weight, and volume, see the Apple Event Manager and Open Scripting Architecture header files.

## Topics

### Constants

var typeSInt16: DescType

16-bit signed integer.

var typeUInt16: DescType

16-bit unsigned integer.

var typeSInt32: DescType

32-bit signed integer.

var typeUInt32: DescType

32-bit unsigned integer.

var typeSInt64: DescType

64-bit signed integer.

var typeUInt64: DescType

64-bit unsigned integer.

var typeIEEE32BitFloatingPoint: DescType

32-bit floating point value.

var typeIEEE64BitFloatingPoint: DescType

64-bit floating point value.

var type128BitFloatingPoint: DescType

128-bit floating point value.

var typeDecimalStruct: DescType

Decimal.

