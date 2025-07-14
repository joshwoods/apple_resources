

- Video Toolbox
-  VTSessionCopySupportedPropertyDictionary(\_:supportedPropertyDictionaryOut:) 

Function

# VTSessionCopySupportedPropertyDictionary(\_:supportedPropertyDictionaryOut:)

Retrieves a dictionary enumerating all the supported properties of a video toolbox session.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTSessionCopySupportedPropertyDictionary(
    _ session: VTSession,
    supportedPropertyDictionaryOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`session`  

The session object.

`supportedPropertyDictionaryOut`  

A pointer to a doc://com.apple.documentation/documentation/corefoundation/cfdictionary-rum.

## Discussion

The keys of the returned dictionary are the supported property keys.

The values are themselves dictionaries, each containing the following optional fields:

- The type of value (kVTPropertyTypeKey)

- The read/write status of the property (kVTPropertyReadWriteStatusKey)

- Whether the property is suitable for serialization (kVTPropertyShouldBeSerializedKey)

- A range or list of the supported values, if appropriate

- Developer-level documentation for the property (kVTPropertyDocumentationKey)

The caller must release the returned dictionary.

## See Also

### Getting Properties

func VTSessionCopyProperty(VTSession, key: CFString, allocator: CFAllocator?, valueOut: UnsafeMutableRawPointer?) -> OSStatus

Retrieves a property on a Video Toolbox session.

func VTSessionCopySerializableProperties(VTSession, allocator: CFAllocator?, dictionaryOut: UnsafeMutablePointer&lt;CFDictionary?>) -> OSStatus

Retrieves the set of serializable property keys and their current values.

Supported Property Dictionary Constants

Property dictionary key and constant values.

