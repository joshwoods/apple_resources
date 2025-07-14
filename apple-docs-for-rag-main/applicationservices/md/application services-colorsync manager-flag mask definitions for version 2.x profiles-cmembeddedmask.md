

- Application Services
- ColorSync Manager
- Flag Mask Definitions for Version 2.x Profiles
-  cmEmbeddedMask 

Global Variable

# cmEmbeddedMask

This mask provides access to bit 0 of the `flags` field, which specifies whether the profile is embedded. It has the value 1 if the profile is embedded, 0 if it is not.

macOS 10.0+

``` source
var cmEmbeddedMask: Int { get }
```

