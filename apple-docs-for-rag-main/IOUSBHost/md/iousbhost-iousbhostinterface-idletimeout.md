

- IOUSBHost
- IOUSBHostInterface
-  idleTimeout 

Instance Property

# idleTimeout

The current idle suspend timeout.

Mac Catalyst 14.0+macOS 10.15+

``` source
var idleTimeout: TimeInterval { get }
```

## Return Value

The amount of time after all pipes are idle to wait before suspending the device.

## See Also

### Enabling Power Savings

func setIdleTimeout(TimeInterval) throws

Sets the desired idle suspend timeout for the interface.

