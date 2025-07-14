

- Video Toolbox
-  VTSessionSetProperty(\_:key:value:) 

Function

# VTSessionSetProperty(\_:key:value:)

Sets a property on a VideoToolbox session.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.8+tvOS 10.2+visionOS 1.0+

``` source
func VTSessionSetProperty(
    _ session: VTSession,
    key propertyKey: CFString,
    value propertyValue: CFTypeRef?
) -> OSStatus
```

## Discussion

Setting a property value to `NULL` restores the default value.

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

func VTSessionSetProperties(VTSession, propertyDictionary: CFDictionary) -> OSStatus

Sets multiple properties at once.

