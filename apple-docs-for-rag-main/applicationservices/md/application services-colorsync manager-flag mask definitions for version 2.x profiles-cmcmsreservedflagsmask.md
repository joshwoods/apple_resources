

- Application Services
- ColorSync Manager
- Flag Mask Definitions for Version 2.x Profiles
-  cmCMSReservedFlagsMask 

Global Variable

# cmCMSReservedFlagsMask

macOS 10.0+

``` source
var cmCMSReservedFlagsMask: Int { get }
```

## Discussion

This mask provides access to bits 16 through 31 of the `flags` field, which are available for a color management system (CMS) vendor, such as ColorSync. ColorSync’s default CMM uses bits 16 through 19 to provide hints for color matching, as described in the following three mask definitions. Other CMM vendors should follow the same conventions.

