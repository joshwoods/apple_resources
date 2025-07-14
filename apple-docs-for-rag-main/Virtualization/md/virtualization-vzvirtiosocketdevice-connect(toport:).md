

- Virtualization
- VZVirtioSocketDevice
-  connect(toPort:) 

Instance Method

# connect(toPort:)

Initiates a connection to the specified port of the guest operating system.

macOS 11.0+

``` source
func connect(toPort port: UInt32) async throws -> VZVirtioSocketConnection
```

## Parameters 

`port`  

The destination port number in the guest operating system.

## Discussion

This method initiates the connection asynchronously, and executes the completion handler when the results are available. If the guest operating system doesn’t listen for connections to the specifed port, this method does nothing.

For a successful connection, this method sets the sourcePort property of the resulting VZVirtioSocketConnection object to a random port number.

## See Also

### Connecting to Guest System Ports

func connect(toPort: UInt32, completionHandler: (Result&lt;VZVirtioSocketConnection, any Error>) -> Void)

Initiates a connection to the specified port of the guest operating system.

