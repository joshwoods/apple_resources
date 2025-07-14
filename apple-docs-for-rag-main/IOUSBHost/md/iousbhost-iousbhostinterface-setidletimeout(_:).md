

- IOUSBHost
- IOUSBHostInterface
-  setIdleTimeout(\_:) 

Instance Method

# setIdleTimeout(\_:)

Sets the desired idle suspend timeout for the interface.

Mac Catalyst 14.0+macOS 10.15+

``` source
func setIdleTimeout(_ idleTimeout: TimeInterval) throws
```

## Parameters 

`idleTimeout`  

The amount of time after all pipes are idle to wait before suspending the device.

## Discussion

After the interface idles, it defers electrical suspension of the device for the specified duration.

## See Also

### Enabling Power Savings

var idleTimeout: TimeInterval

The current idle suspend timeout.

