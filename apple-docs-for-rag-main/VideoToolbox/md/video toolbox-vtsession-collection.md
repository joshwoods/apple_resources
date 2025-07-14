

- Video Toolbox
-  VTSession 

API Collection

# VTSession

An abstract object that provides the common interface to configure VideoToolbox session objects.

## Topics

### Setting Properties

func VTSessionSetProperty(VTSession, key: CFString, value: CFTypeRef?) -> OSStatus

Sets a property on a VideoToolbox session.

func VTSessionSetProperties(VTSession, propertyDictionary: CFDictionary) -> OSStatus

Sets multiple properties at once.

### Getting Properties

func VTSessionCopyProperty(VTSession, key: CFString, allocator: CFAllocator?, valueOut: UnsafeMutableRawPointer?) -> OSStatus

Retrieves a property on a Video Toolbox session.

func VTSessionCopySerializableProperties(VTSession, allocator: CFAllocator?, dictionaryOut: UnsafeMutablePointer&lt;CFDictionary?>) -> OSStatus

Retrieves the set of serializable property keys and their current values.

func VTSessionCopySupportedPropertyDictionary(VTSession, supportedPropertyDictionaryOut: UnsafeMutablePointer&lt;CFDictionary?>) -> OSStatus

Retrieves a dictionary enumerating all the supported properties of a video toolbox session.

Supported Property Dictionary Constants

Property dictionary key and constant values.

### Data Types

typealias VTSession

A reference to a VideoToolbox compression session, decompression session or pixel transfer session.

### Enumerations

Frame Delay

Indicates that no limit should be placed on the compression window.

## See Also

### Data Types

struct VTInt32Point

A structure that represents a 32-bit integer point value.

struct VTInt32Size

A structure that represents a 32-bit integer size value.

var VT_SUPPORT_COLORSYNC_PIXEL_TRANSFER: Bool

