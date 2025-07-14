

- Video Toolbox
-  VTSessionSetProperties(\_:propertyDictionary:) 

Function

# VTSessionSetProperties(\_:propertyDictionary:)

Sets multiple properties at once.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTSessionSetProperties(
    _ session: VTSession,
    propertyDictionary: CFDictionary
) -> OSStatus
```

## Discussion

Sets the properties specified by keys in `propertyDictionary` to the corresponding values.

## Topics

### Related Documentation

Compression Properties

Properties that you use to configure a compression session.

Decompression Properties

Properties used to configure a VideoToolbox decompression session.

Pixel Transfer Properties

Properties used to configure a VideoToolbox pixel transfer session.

## See Also

### Setting Properties

func VTSessionSetProperty(VTSession, key: CFString, value: CFTypeRef?) -> OSStatus

Sets a property on a VideoToolbox session.

