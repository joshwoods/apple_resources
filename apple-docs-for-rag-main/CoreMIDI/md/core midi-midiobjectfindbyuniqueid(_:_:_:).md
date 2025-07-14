

- Core MIDI
-  MIDIObjectFindByUniqueID(\_:\_:\_:) 

Function

# MIDIObjectFindByUniqueID(\_:\_:\_:)

Locates a device, entity, or endpoint by its unique identifier.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
func MIDIObjectFindByUniqueID(
    _ inUniqueID: MIDIUniqueID,
    _ outObject: UnsafeMutablePointer?,
    _ outObjectType: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`inUniqueID`  

The unique ID of the object to search for. You determine the unique ID by querying MIDIObjectGetIntegerProperty(_:_:_:) for the kMIDIPropertyUniqueID property.

`outObject`  

The returned object, or 0 if the object wasn’t found or an error occurred. Cast this pointer to the appropriate type, according to type specified by the `outObjectType` argument.

`outObjectType`  

On exit, the type of object found, or undefined if the system found no objects.

## Return Value

An `OSStatus` error code, including kMIDIObjectNotFound if there is no object with this unique ID.

## Topics

### Parameter Types

typealias MIDIUniqueID

A MIDI object’s unique identifier.

var kMIDIInvalidUniqueID: MIDIUniqueID

An invalid identifier.

enum MIDIObjectType

The MIDI object types that the system supports.

## See Also

### MIDI object configuration

typealias MIDIObjectRef

The common base class for many of the framework’s objects.

MIDI Object Properties

Configure the properties of MIDI objects.

