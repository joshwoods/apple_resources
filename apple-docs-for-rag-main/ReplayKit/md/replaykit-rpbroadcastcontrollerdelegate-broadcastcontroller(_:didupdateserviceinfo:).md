

- ReplayKit
- RPBroadcastControllerDelegate
-  broadcastController(\_:didUpdateServiceInfo:) 

Instance Method

# broadcastController(\_:didUpdateServiceInfo:)

Tells the delegate the broadcast service has data to pass back to the broadcasting app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
optional func broadcastController(
    _ broadcastController: RPBroadcastController,
    didUpdateServiceInfo serviceInfo: [String : any NSCoding & NSObjectProtocol]
)
```

**Required**

## Parameters 

`broadcastController`  

The RPBroadcastController instance.

`serviceInfo`  

Dictionary that is passed back to the broadcasting app and contains information about the ongoing broadcast.

## See Also

### Updating a Broadcast

func broadcastController(RPBroadcastController, didUpdateBroadcast: URL)

Tells the broadcast service the broadcast URL has been updated.

