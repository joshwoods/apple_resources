

- Virtualization
- VZVirtioSocketDevice
-  connect(toPort:completionHandler:) 

Instance Method

# connect(toPort:completionHandler:)

Initiates a connection to the specified port of the guest operating system.

macOS 11.0+

``` source
func connect(
    toPort port: UInt32,
    completionHandler: @escaping (Result) -> Void
)
```

## Parameters 

`port`  

The destination port number in the guest operating system.

`completionHandler`  

The block to execute with the results of the connection attempt. This block has no return value and takes the following parameter:

result  
The result of the connection attempt. On a successful attempt, this value is the VZVirtioSocketConnection object to use for communications. On an unsuccessful attempt, this value is the error object that indicates why the connection failed.

## Discussion

This method initiates the connection asynchronously, and executes the completion handler when the results are available. If the guest operating system doesn’t listen for connections to the specifed port, this method does nothing.

For a successful connection, this method sets the sourcePort property of the resulting VZVirtioSocketConnection object to a random port number.

## See Also

### Connecting to Guest System Ports

func connect(toPort: UInt32) async throws -> VZVirtioSocketConnection

Initiates a connection to the specified port of the guest operating system.

