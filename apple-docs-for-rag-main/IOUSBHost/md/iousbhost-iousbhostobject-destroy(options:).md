

- IOUSBHost
- IOUSBHostObject
-  destroy(options:) 

Instance Method

# destroy(options:)

Mac Catalyst 14.0+macOS 10.15+

``` source
func destroy(options: IOUSBHostObjectDestroyOptions = [])
```

## Discussion

```
         IOUSBHostObjectDestroyOptionsDeviceSurrender is defined to support surrendering ownersip of
         the kernel service.  To be used when accepting the kUSBHostMessageDeviceIsRequestingClose message.
```

