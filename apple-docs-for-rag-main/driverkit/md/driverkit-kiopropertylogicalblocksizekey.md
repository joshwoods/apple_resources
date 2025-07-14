

- DriverKit
-  kIOPropertyLogicalBlockSizeKey 

Macro

# kIOPropertyLogicalBlockSizeKey

DriverKitiOSiPadOSmacOS

``` source
#define kIOPropertyLogicalBlockSizeKey
```

## Discussion

This key is used to define the logical block size of a hard disk drive.

Requirement: Mandatory for hard disk drives with logical block size other than 512 bytes or that does not match its physical block size.

Example:

```

   Device Characteristics

       Vendor Name
       Apple
       Product Name
       iPod
       Product Revision Level
       1.0
       Physical Block Size
       4096
       Logical Block Size
       512

```

## See Also

### Macros

ALWAYS

APPLE_KEXT_OVERRIDE

DEFN

DRIVERKIT_CONSUMED

DRIVERKIT_CONSUMES_THIS

DRIVERKIT_FRAMEWORK_INCLUDE

DRIVERKIT_IOLIB_H

DRIVERKIT_OSCOLLECTIONS_H

DRIVERKIT_RETURNS_NOT_RETAINED

DRIVERKIT_RETURNS_RETAINED

DRIVERKIT_RETURNS_RETAINED_ON_NONZERO

DRIVERKIT_RETURNS_RETAINED_ON_ZERO

ERR_SUCCESS

EXTENDS

HIDDEN

