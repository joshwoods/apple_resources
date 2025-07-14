

- Foundation
- NSXPCInterface
-  setInterface(\_:for:argumentIndex:ofReply:) 

Instance Method

# setInterface(\_:for:argumentIndex:ofReply:)

Configures a specific parameter of a method to be sent as a proxy object instead of copied.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setInterface(
    _ ifc: NSXPCInterface,
    for sel: Selector,
    argumentIndex arg: Int,
    ofReply: Bool
)
```

## Parameters 

`ifc`  

The NSXPCInterface object that describes the protocol for the proxy object. The interface is configured the same way as the interface for an exported object or remote object proxy.

`sel`  

Specifies which method in the protocol is being configured.

`arg`  

Specifies the position (starting at index 0) of the parameter for which you are configuring a proxy object. This may be either the position of a parameter in the method itself or the position in its reply block. This argument must be an object.

`ofReply`  

Pass true if `arg` is an index into the parameters of the reply block, or false if it is an index into the parameters of the method itself.

## Discussion

If an argument to a method in your protocol should be sent as a proxy object instead of by copy, then configure the interface for that protocol with a new interface for a specific argument. An example of an object that should be a proxy instead of being copied is a view object.

