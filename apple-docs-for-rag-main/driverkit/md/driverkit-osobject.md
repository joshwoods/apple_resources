

- DriverKit
-  OSObject 

Class

# OSObject

The base class for DriverKit objects

DriverKitiOSiPadOSmacOS

``` source
class OSObject;
```

## Topics

### Managing the Object Lifecycle

init

retain

Retains the OSObject instance

release

Releases the OSObject instance

free

OSObjectPtr

OSObjectRef

### Managing an Object’s Dispatch Queue

SetDispatchQueue

CopyDispatchQueue

## Relationships

### Inherits From

- OSMetaClassBase

### Inherited By

- IOCommand
- IOCommandPool
- IODMACommand
- IODispatchQueue
- IODispatchSource
- IOMemoryDescriptor
- IOMemoryMap
- IOReportLegend
- IOReporter
- IOService
- OSAction
- OSBundle
- OSContainer
- OSMappedFile

## See Also

### Registry data types

OSArray

A container for an ordered, random-access collection of objects.

OSDictionary

A container for a collection with elements that are key-value pairs.

OSBoolean

A container for a true or false value.

OSData

A container for untyped data.

OSNumber

A container for an integer value.

OSString

A container for managing an array of characters.

OSSerialization

A container for one or more objects, serialized in a binary data format that is suitable for messaging.

OSCollection

The base class for DriverKit collection objects.

OSContainer

The base class for DriverKit data objects.

OSSymbol

A container for managing an array of characters.

IOFixed

A fixed-point number.

