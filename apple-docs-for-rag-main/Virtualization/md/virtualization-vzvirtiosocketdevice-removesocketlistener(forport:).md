

- Virtualization
- VZVirtioSocketDevice
-  removeSocketListener(forPort:) 

Instance Method

# removeSocketListener(forPort:)

Removes the listener object from the specfied port.

macOS 11.0+

``` source
func removeSocketListener(forPort port: UInt32)
```

## Parameters 

`port`  

The port number to clear. If the specified port doesn’t have a listener object, this method does nothing.

## See Also

### Configuring Port Listeners

func setSocketListener(VZVirtioSocketListener, forPort: UInt32)

Configures an object to monitor the specified port for new connections.

