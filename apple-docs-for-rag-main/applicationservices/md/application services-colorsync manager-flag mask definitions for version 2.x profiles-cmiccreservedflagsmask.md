

- Application Services
- ColorSync Manager
- Flag Mask Definitions for Version 2.x Profiles
-  cmICCReservedFlagsMask 

Global Variable

# cmICCReservedFlagsMask

macOS 10.0+

``` source
var cmICCReservedFlagsMask: Int { get }
```

## Discussion

This mask provides access to bits 0 through 15 of the `flags` field, which are defined and reserved by the ICC. For more information, see the International Color Consortium Profile Format Specification, and the next two mask definitions.

To obtain a copy of the ICC specification, or to get other information about the ICC, visit the ICC Web site at http://www.color.org/.

