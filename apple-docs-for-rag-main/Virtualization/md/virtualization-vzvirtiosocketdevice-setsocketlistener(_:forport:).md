

- Virtualization
- VZVirtioSocketDevice
-  setSocketListener(\_:forPort:) 

Instance Method

# setSocketListener(\_:forPort:)

Configures an object to monitor the specified port for new connections.

macOS 11.0+

``` source
func setSocketListener(
    _ listener: VZVirtioSocketListener,
    forPort port: UInt32
)
```

## Parameters 

`listener`  

The VZVirtioSocketListener object to monitor the port. This object replaces the previous listener object, if any.

`port`  

The port number to monitor.

## Discussion

You can register the same listener object on multiple ports. When the guest operating system opens a connection to the port, the listener object notifies its associated delegate.

## See Also

### Configuring Port Listeners

func removeSocketListener(forPort: UInt32)

Removes the listener object from the specfied port.

