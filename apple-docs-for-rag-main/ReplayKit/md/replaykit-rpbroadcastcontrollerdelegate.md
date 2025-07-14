

- ReplayKit
-  RPBroadcastControllerDelegate 

Protocol

# RPBroadcastControllerDelegate

The protocol you implement to respond to changes in a live broadcast.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
protocol RPBroadcastControllerDelegate : NSObjectProtocol
```

## Topics

### Finishing a Broadcast

func broadcastController(RPBroadcastController, didFinishWithError: (any Error)?)

Tells the delegate that a broadcast ended due to an error.

**Required**

### Updating a Broadcast

func broadcastController(RPBroadcastController, didUpdateServiceInfo: [String : any NSCoding &amp; NSObjectProtocol])

Tells the delegate the broadcast service has data to pass back to the broadcasting app.

**Required**

func broadcastController(RPBroadcastController, didUpdateBroadcast: URL)

Tells the broadcast service the broadcast URL has been updated.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Getting the Delegate

var delegate: (any RPBroadcastControllerDelegate)?

The delegate for the broadcast controller.

