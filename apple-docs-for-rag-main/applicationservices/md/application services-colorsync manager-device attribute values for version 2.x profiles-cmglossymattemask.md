

- Application Services
- ColorSync Manager
- Device Attribute Values for Version 2.x Profiles
-  cmGlossyMatteMask 

Global Variable

# cmGlossyMatteMask

macOS 10.0+

``` source
var cmGlossyMatteMask: Int { get }
```

## Discussion

Bit 1of `deviceAttributes[1]` specifies whether the media is glossy or matte. If it has the value 0, the media is glossy; if it has the value 1, the media is matte. Use the `cmGlossyMatteMask` mask to set the glossy/matte bit in `deviceAttributes[1]` or to clear all bits except the glossy/matte bit.

