

- Core MIDI
-  MIDIObjectRemoveProperty(\_:\_:) 

Function

# MIDIObjectRemoveProperty(\_:\_:)

Removes an object’s property.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
func MIDIObjectRemoveProperty(
    _ obj: MIDIObjectRef,
    _ propertyID: CFString
) -> OSStatus
```

## Parameters 

`obj`  

The object to modify,

`propertyID`  

The property to remove.

## Return Value

An `OSStatus` result code.

## See Also

### Property Accessors

func MIDIObjectGetProperties(MIDIObjectRef, UnsafeMutablePointer&lt;Unmanaged&lt;CFPropertyList>?>, Bool) -> OSStatus

Returns all properties of an object.

func MIDIObjectGetStringProperty(MIDIObjectRef, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>) -> OSStatus

Gets an object’s string-type property.

func MIDIObjectSetStringProperty(MIDIObjectRef, CFString, CFString) -> OSStatus

Sets an object’s string-type property.

func MIDIObjectGetIntegerProperty(MIDIObjectRef, CFString, UnsafeMutablePointer&lt;Int32>) -> OSStatus

Gets an object’s integer-type property.

func MIDIObjectSetIntegerProperty(MIDIObjectRef, CFString, Int32) -> OSStatus

Sets an object’s integer-type property.

func MIDIObjectGetDataProperty(MIDIObjectRef, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>) -> OSStatus

Gets an object’s data-type property.

func MIDIObjectSetDataProperty(MIDIObjectRef, CFString, CFData) -> OSStatus

Sets an object’s data-type property.

func MIDIObjectGetDictionaryProperty(MIDIObjectRef, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

Gets an object’s dictionary-type property.

func MIDIObjectSetDictionaryProperty(MIDIObjectRef, CFString, CFDictionary) -> OSStatus

Sets an object’s dictionary-type property.

