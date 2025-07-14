

- Video Toolbox
- VTSession
-  Supported Property Dictionary Constants 

API Collection

# Supported Property Dictionary Constants

Property dictionary key and constant values.

## Overview

Property dictionary key and constant values for a dictionary populated by VTSessionCopySupportedPropertyDictionary(_:supportedPropertyDictionaryOut:).

## Topics

### Properties

let kVTPropertyTypeKey: CFString

Dictionary key used to access the property type.

Property Type Constants

Supported constant values for `kVTPropertyTypeKey`.

let kVTPropertyReadWriteStatusKey: CFString

Dictionary key to access the read/write status of a property.

Read/Write Status Constants

Supported constant values for `kVTPropertyReadWriteStatusKey`.

let kVTPropertyShouldBeSerializedKey: CFString

Dictionary key to access the serializable status of a property.

let kVTPropertySupportedValueListKey: CFString

Dictionary key to access the array of of supported values.

let kVTPropertySupportedValueMaximumKey: CFString

Dictionary key to access the maximum value of a property.

let kVTPropertySupportedValueMinimumKey: CFString

Dictionary key to access the minimum value of a property.

let kVTPropertyDocumentationKey: CFString

Dictionary key to access any documentation intended for developers only.

## See Also

### Getting Properties

func VTSessionCopyProperty(VTSession, key: CFString, allocator: CFAllocator?, valueOut: UnsafeMutableRawPointer?) -> OSStatus

Retrieves a property on a Video Toolbox session.

func VTSessionCopySerializableProperties(VTSession, allocator: CFAllocator?, dictionaryOut: UnsafeMutablePointer&lt;CFDictionary?>) -> OSStatus

Retrieves the set of serializable property keys and their current values.

func VTSessionCopySupportedPropertyDictionary(VTSession, supportedPropertyDictionaryOut: UnsafeMutablePointer&lt;CFDictionary?>) -> OSStatus

Retrieves a dictionary enumerating all the supported properties of a video toolbox session.

