

- Installer JS
- Applications
-  fromIdentifier 

# fromIdentifier

Provides information about running processes with a given application identifier (bundle ID).

``` source
fromIdentifier(bundleID)
```

## Parameters 

`bundleID`  

A string with the bundle ID of the desired application, such as `com.apple.TextEdit`.

## Return Value

An array of dictionaries (associative arrays) describing the running applications identified by `bundleID`.

## See Also

### Getting Information About Running Applications

fromPID

Provides information about a running application with a given process ID.

all

All running applications registered with the process manager.

### Related Documentation

ProcessInformation

A dictionary (associative array) describing an application.

