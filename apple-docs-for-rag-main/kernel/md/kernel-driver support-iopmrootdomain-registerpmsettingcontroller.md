

- Kernel
- Driver Support
- IOPMrootDomain
-  registerPMSettingController 

Instance Method

# registerPMSettingController

macOS 10.15.2+

``` source
IOReturn registerPMSettingController(const OSSymbol *settings[], uint32_t supportedPowerSources, IOPMSettingControllerCallback callout, OSObject *target, uintptr_t refcon, OSObject **handle);
```

