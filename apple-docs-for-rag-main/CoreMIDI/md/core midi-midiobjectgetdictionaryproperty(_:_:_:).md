

- Core MIDI
-  MIDIObjectGetDictionaryProperty(\_:\_:\_:) 

Function

# MIDIObjectGetDictionaryProperty(\_:\_:\_:)

Gets an object’s dictionary-type property.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.2+visionOS 1.0+

``` source
func MIDIObjectGetDictionaryProperty(
    _ obj: MIDIObjectRef,
    _ propertyID: CFString,
    _ outDict: UnsafeMutablePointer?>
) -> OSStatus
```

## Parameters 

`obj`  

The object to query.

`propertyID`  

The name of the property to return.

`outDict`  

On successful return, the property value.

## Return Value

An `OSStatus` result code.

## Discussion

See MIDIObjectRef for information about properties.

## See Also

### Property Accessors

func MIDIObjectGetProperties(MIDIObjectRef, UnsafeMutablePointer&lt;Unmanaged&lt;CFPropertyList>?>, Bool) -> OSStatus

Returns all properties of an object.

func MIDIObjectRemoveProperty(MIDIObjectRef, CFString) -> OSStatus

Removes an object’s property.

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

func MIDIObjectSetDictionaryProperty(MIDIObjectRef, CFString, CFDictionary) -> OSStatus

Sets an object’s dictionary-type property.

