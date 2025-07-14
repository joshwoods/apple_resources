

- Application Services
- ColorSync Manager
- Device Attribute Values for Version 2.x Profiles
-  cmReflectiveTransparentMask 

Global Variable

# cmReflectiveTransparentMask

macOS 10.0+

``` source
var cmReflectiveTransparentMask: Int { get }
```

## Discussion

Bit 0 of `deviceAttributes[1]` specifies whether the media is transparent or reflective. If it has the value 0, the media is reflective; if it has the value 1, the media is transparent. Use the `cmReflectiveTransparentMask` mask to set the transparent/reflective bit in `deviceAttributes[1]` or to clear all bits except the transparent/reflective bit.

