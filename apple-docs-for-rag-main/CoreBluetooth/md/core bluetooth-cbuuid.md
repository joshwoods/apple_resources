

- Core Bluetooth
-  CBUUID 

Class

# CBUUID

A universally unique identifier, as defined by Bluetooth standards.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class CBUUID
```

## Overview

Instances of the CBUUID class represent the 128-bit universally unique identifiers (UUIDs) of attributes used in Bluetooth low energy communication, such as a peripheral’s services, characteristics, and descriptors. This class provides a number of factory methods for dealing with long UUIDs when developing your app. For example, instead of passing around the string representation of a 128-bit Bluetooth low energy attribute in your code, you can create a CBUUID object that represents it, and pass that around instead.

The Bluetooth Special Interest Group (SIG) publishes a list of commonly-used UUIDs, many of which are 16- or 32-bits for convenience. The CBUUID class provides methods that automatically transform these predefined shorter UUIDs into their 128-bit equivalent UUIDs. When you create a CBUUID object from a predefined 16- or 32-bit UUID, Core Bluetooth pre-fills the rest of the 128-bit UUID with the Bluetooth base UUID, as defined in the Bluetooth 4.0 specification, Volume 3, Part F, Section 3.2.1.

In addition to providing methods for creating CBUUID objects, this class defines constants that represent the UUIDs of the Bluetooth-defined characteristic descriptors, as defined in the Bluetooth 4.0 specification, Volume 3, Part G, Section 3.3.3.

## Topics

### Creating New CBUUID Objects

init(string: String)

Creates a Core Bluetooth UUID object from a 16-, 32-, or 128-bit UUID string.

init(data: Data)

Creates a Core Bluetooth UUID object from a 16-, 32-, or 128-bit UUID data container.

init(cfuuid: CFUUID)

Creates a Core Bluetooth UUID object from a Core Foundation UUID object.

Deprecated

init(nsuuid: UUID)

Creates a Core Bluetooth UUID object from a Foundation UUID object.

### Inspecting CBUUID Properties

var data: Data

The data of the UUID.

var uuidString: String

The UUID represented as a string.

### UUID Constants

Characteristic Descriptors

Values that represent the UUIDs of the characteristic descriptors.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Supporting Types

class CBManager

The abstract base class that manages central and peripheral objects.

class CBATTRequest

A request that uses the Attribute Protocol (ATT).

class CBPeer

An object that represents a remote device.

