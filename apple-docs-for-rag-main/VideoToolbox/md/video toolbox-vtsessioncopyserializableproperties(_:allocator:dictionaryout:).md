

- Video Toolbox
-  VTSessionCopySerializableProperties(\_:allocator:dictionaryOut:) 

Function

# VTSessionCopySerializableProperties(\_:allocator:dictionaryOut:)

Retrieves the set of serializable property keys and their current values.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTSessionCopySerializableProperties(
    _ session: VTSession,
    allocator: CFAllocator?,
    dictionaryOut: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`session`  

The session object.

`allocator`  

An allocator suitable for use when copying property values.

`dictionaryOut`  

A pointer to the properties dictionary.

## Discussion

The serializable properties are those which can be saved and applied to a different session. The caller must release the returned dictionary.

## See Also

### Getting Properties

func VTSessionCopyProperty(VTSession, key: CFString, allocator: CFAllocator?, valueOut: UnsafeMutableRawPointer?) -> OSStatus

Retrieves a property on a Video Toolbox session.

func VTSessionCopySupportedPropertyDictionary(VTSession, supportedPropertyDictionaryOut: UnsafeMutablePointer&lt;CFDictionary?>) -> OSStatus

Retrieves a dictionary enumerating all the supported properties of a video toolbox session.

Supported Property Dictionary Constants

Property dictionary key and constant values.

