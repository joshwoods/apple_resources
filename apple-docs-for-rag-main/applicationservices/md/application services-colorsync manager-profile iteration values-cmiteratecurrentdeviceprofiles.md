

- Application Services
- ColorSync Manager
- Profile Iteration Values
-  cmIterateCurrentDeviceProfiles 

Global Variable

# cmIterateCurrentDeviceProfiles

macOS 10.0+

``` source
var cmIterateCurrentDeviceProfiles: Int { get }
```

## Discussion

Iterate profiles registered through the routing `CMSetDeviceProfiles`. To get the profiles in use for all devices, use `cmIterateCurrentDeviceProfiles` as the flags value. This will replace the factory profiles with any overrides, yielding the currently used set.I

