

- Application Services
- ColorSync Manager
- Profile Iteration Values
-  cmIterateFactoryDeviceProfiles 

Global Variable

# cmIterateFactoryDeviceProfiles

Iterate profiles registered through the routine `CMSetDeviceFactoryProfiles`. To retrieve all factory profiles for all devices, use `cmIterateFactoryDeviceProfiles` as the flags value when calling `CMIterateDeviceProfiles`. I

macOS 10.0+

``` source
var cmIterateFactoryDeviceProfiles: Int { get }
```

