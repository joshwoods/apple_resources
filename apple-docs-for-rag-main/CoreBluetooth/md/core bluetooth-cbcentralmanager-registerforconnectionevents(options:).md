

- Core Bluetooth
- CBCentralManager
-  registerForConnectionEvents(options:) 

Instance Method

# registerForConnectionEvents(options:)

Register for an event notification when the central manager makes a connection matching the given options.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func registerForConnectionEvents(options: [CBConnectionEventMatchingOption : Any]? = nil)
```

## Parameters 

`options`  

A dictionary that specifies options for connection events. See Peripheral Connection Options for a list of possible options.

## Discussion

When the central manager makes a connection that matches the options, it calls the delegate’s centralManager(_:connectionEventDidOccur:for:) method.

## See Also

### Receiving Connection Events

Peripheral Connection Options

Keys used to pass options when connecting to a peripheral.

enum CBConnectionEvent

A change to the connection state of a peer.

struct CBConnectionEventMatchingOption

A set of options to use when registering for connection events.

