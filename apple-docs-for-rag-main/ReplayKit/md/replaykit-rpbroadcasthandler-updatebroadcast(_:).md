

- ReplayKit
- RPBroadcastHandler
-  updateBroadcast(\_:) 

Instance Method

# updateBroadcast(\_:)

Sends the current broadcast URL to the broadcast controller.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+tvOS 11.0+visionOS 1.0+

``` source
func updateBroadcast(_ broadcastURL: URL)
```

## Parameters 

`broadcastURL`  

A URL that specifies where the broadcast to be passed to the broadcasting app is contained.

## Discussion

This method updates the broadcastURL property for the broadcast controller.

## See Also

### Updating Current Broadcast Information

func updateServiceInfo([String : any NSCoding &amp; NSObjectProtocol])

Sends information about the current broadcast to the broadcasting app.

