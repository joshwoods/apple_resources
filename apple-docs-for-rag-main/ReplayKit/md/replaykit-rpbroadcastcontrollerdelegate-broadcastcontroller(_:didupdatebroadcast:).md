

- ReplayKit
- RPBroadcastControllerDelegate
-  broadcastController(\_:didUpdateBroadcast:) 

Instance Method

# broadcastController(\_:didUpdateBroadcast:)

Tells the broadcast service the broadcast URL has been updated.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+tvOS 11.0+visionOS 1.0+

``` source
optional func broadcastController(
    _ broadcastController: RPBroadcastController,
    didUpdateBroadcast broadcastURL: URL
)
```

## Parameters 

`broadcastController`  

The broadcast controller instance.

`broadcastURL`  

The URL of the resource where the broadcast can be viewed.

## See Also

### Updating a Broadcast

func broadcastController(RPBroadcastController, didUpdateServiceInfo: [String : any NSCoding &amp; NSObjectProtocol])

Tells the delegate the broadcast service has data to pass back to the broadcasting app.

**Required**

