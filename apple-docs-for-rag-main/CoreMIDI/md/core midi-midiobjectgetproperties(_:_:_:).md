

- Core MIDI
-  MIDIObjectGetProperties(\_:\_:\_:) 

Function

# MIDIObjectGetProperties(\_:\_:\_:)

Returns all properties of an object.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.1+visionOS 1.0+

``` source
func MIDIObjectGetProperties(
    _ obj: MIDIObjectRef,
    _ outProperties: UnsafeMutablePointer?>,
    _ deep: Bool
) -> OSStatus
```

## Parameters 

`obj`  

The object to query.

`outProperties`  

On successful return, the object’s properties.

`deep`  

Specify `true` to include the object’s children; for example, a device’s entities, or an entity’s endpoints.

## Return Value

An `OSStatus` result code.

## Discussion

The property list may be a dictionary or an array. Dictionaries map property names (doc://com.apple.documentation/documentation/corefoundation/cfstring-rfh) to values, which may be CFNumber, CFString, or CFData. Arrays provide collections of other property list types.

Properties that an object inherits from its owning object aren’t included.

## See Also

### Property Accessors

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

func MIDIObjectGetDictionaryProperty(MIDIObjectRef, CFString, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> OSStatus

Gets an object’s dictionary-type property.

func MIDIObjectSetDictionaryProperty(MIDIObjectRef, CFString, CFDictionary) -> OSStatus

Sets an object’s dictionary-type property.

