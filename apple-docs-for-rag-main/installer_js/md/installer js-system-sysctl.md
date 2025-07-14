

- Installer JS
- System
-  sysctl 

# sysctl

Provides the result of a `sysctlbyname()` call using the given selector.

``` source
sysctl(selector)
```

## Parameters 

`selector`  

String with the hardware selector for the desired data.

## Return Value

Hardware data corresponding to `selector`.

## Overview

Use `man sysctl` in the macOS Terminal application to see a list of hardware selectors.

Tip

If you are using this function to screen for hardware features at install-time, consider using the “Pre-install Requirements Property List” setting of `productbuild` instead. Use `man productbuild` in the macOS Terminal application to see a list of supported requirement keys.

## See Also

### Accessing System Information

users.desktopSessionCount

The number of logged-in users.

version

A dictionary (associative array) with information about the current system version.

