

- DriverKit
-  kIOPropertyDeviceCharacteristicsKey 

Macro

# kIOPropertyDeviceCharacteristicsKey

DriverKitiOSiPadOSmacOS

``` source
#define kIOPropertyDeviceCharacteristicsKey
```

## Discussion

This key is used to define Device Characteristics for a particular device and it has an associated dictionary which lists the device characteristics. The device characteristics are Command Set specific and are listed in the header files for each command set.

Requirement: Mandatory

Example:

```

   Device Characteristics

       Vendor Name
       Apple
       Product Name
       iPod
       Product Revision Level
       1.0

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

