

- DriverKit
-  kIOPropertySectorCountPerTrackKey 

Macro

# kIOPropertySectorCountPerTrackKey

DriverKitiOSiPadOSmacOS

``` source
#define kIOPropertySectorCountPerTrackKey
```

## Discussion

This key is used to define the number of sectors per each track for a particular medium.

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

