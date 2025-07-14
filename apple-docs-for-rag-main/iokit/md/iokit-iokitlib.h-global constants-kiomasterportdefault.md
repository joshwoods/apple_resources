

- IOKit
- IOKitLib.h
- Global Constants
-  kIOMasterPortDefault 

Global Variable

# kIOMasterPortDefault

The default mach port used to initiate communication with IOKit.

Mac Catalyst 10.14+macOS 10.0–12.0Deprecated

``` source
let kIOMasterPortDefault: mach_port_t
```

## Discussion

When specifying a primary port to IOKit functions, the NULL argument indicates "use the default". This is a synonym for NULL, if you'd rather use a named constant.

