

- DriverKit
-  kIOPropertySupportedBDFeaturesKey 

Macro

# kIOPropertySupportedBDFeaturesKey

DriverKitiOSiPadOSmacOS

``` source
#define kIOPropertySupportedBDFeaturesKey
```

## Discussion

This key is used to define the supported BD Features for a particular optical device and it has an associated bitfield. See \ for definitions of the bits and associated bitmasks.

Requirement: Mandatory for optical devices (Peripheral Device Type 05h).

Example:

```

   Device Characteristics

       Vendor Name
       Apple
       Product Name
       SuperDrive
       Product Revision Level
       1.0
       CD Features
       1663
       DVD Features
       103
       BD Features
       21

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

