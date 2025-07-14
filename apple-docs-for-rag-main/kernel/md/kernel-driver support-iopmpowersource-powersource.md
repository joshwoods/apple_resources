

- Kernel
- Driver Support
- IOPMPowerSource
-  powerSource 

# powerSource

Creates a new IOPMPowerSource nub. Must be attached to IORegistry, and registered by provider.

``` source
static IOPMPowerSource *powerSource(
 void); 
```

## See Also

### Miscellaneous

setPSProperty

updateStatus

Must be called by physical battery controller when battery state has changed significantly.

