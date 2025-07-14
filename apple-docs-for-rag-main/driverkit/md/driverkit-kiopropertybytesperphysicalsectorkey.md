

- DriverKit
-  kIOPropertyBytesPerPhysicalSectorKey 

Macro

# kIOPropertyBytesPerPhysicalSectorKey

DriverKitiOSiPadOSmacOS

``` source
#define kIOPropertyBytesPerPhysicalSectorKey
```

## Discussion

This key is used to define the number of heads for a particular medium.

Requirement: Mandatory element of the Rigid Disk Geometry dictionary.

Example:

```

   Device Characteristics

       Vendor Name
       Apple
       Product Name
       iPod
       Product Revision Level
       1.0
       Rigid Disk Geometry

           Sector Count per Track
           12345
           Head Count
           12
           Cylinder Count
           12345
           Bytes per Physical Sector
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

