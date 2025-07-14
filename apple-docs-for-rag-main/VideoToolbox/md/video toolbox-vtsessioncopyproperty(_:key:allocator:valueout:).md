

- Video Toolbox
-  VTSessionCopyProperty(\_:key:allocator:valueOut:) 

Function

# VTSessionCopyProperty(\_:key:allocator:valueOut:)

Retrieves a property on a Video Toolbox session.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTSessionCopyProperty(
    _ session: VTSession,
    key propertyKey: CFString,
    allocator: CFAllocator?,
    valueOut propertyValueOut: UnsafeMutableRawPointer?
) -> OSStatus
```

## Parameters 

`session`  

A Video Toolbox session object.

`propertyKey`  

The key for the property to retrieve.

`allocator`  

An allocator suitable for use when copying property values.

`propertyValueOut`  

Points to a variable to receive the property value, which must be a CF-registered type – the caller may call CFGetTypeID(_:) on it to identify which specific type. The caller must release the this property value.

## Return Value

`noErr` if successful; kVTPropertyNotSupportedErr for unrecognized or unsupported properties.

## Discussion

Note

For most types of properties, the returned values should be considered immutable. In particular, for CFPropertyList types, sharing of mutable property value objects between the client, session and codec should be avoided. However, some properties will be used for exchanging service objects that are inherently mutable (eg, CVPixelBufferPool).

## See Also

### Getting Properties

func VTSessionCopySerializableProperties(VTSession, allocator: CFAllocator?, dictionaryOut: UnsafeMutablePointer&lt;CFDictionary?>) -> OSStatus

Retrieves the set of serializable property keys and their current values.

func VTSessionCopySupportedPropertyDictionary(VTSession, supportedPropertyDictionaryOut: UnsafeMutablePointer&lt;CFDictionary?>) -> OSStatus

Retrieves a dictionary enumerating all the supported properties of a video toolbox session.

Supported Property Dictionary Constants

Property dictionary key and constant values.

