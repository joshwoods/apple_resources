

- Core Services
- Apple Events
-  Other Descriptor Type Constants 

# Other Descriptor Type Constants

Specify types for Boolean and character descriptors.

## Overview

The constants described here specify the data type for a descriptor and show the kind of data stored in a descriptor with that type.

Descriptors are the building blocks used by the Apple Event Manager to construct Apple event attributes and parameters. A descriptor is a data structure of type AEDesc, which consists of data storage and a descriptor type that identifies the type of the data. A descriptor type is defined by the data type DescType.

AppleScript defines descriptor type constants for a wide variety of common data types. For additional types, see Descriptor Type Constants and Numeric Descriptor Type Constants. For a complete listing, including data types such as units of length, weight, and volume, see the Apple Event Manager and Open Scripting Architecture header files.

### Version-Notes

In macOS `typeChar` type is deprecated in favor of `typeUTF8Text` or `typeUTF16ExternalRepresentation`. For more information, see typeUTF16ExternalRepresentation.

## Topics

### Constants

var typeBoolean: DescType

Boolean value—single byte with value 0 or 1.

var typeChar: DescType

