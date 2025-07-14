

- ReplayKit
- RPBroadcastHandler
-  updateServiceInfo(\_:) 

Instance Method

# updateServiceInfo(\_:)

Sends information about the current broadcast to the broadcasting app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
func updateServiceInfo(_ serviceInfo: [String : any NSCoding & NSObjectProtocol])
```

## Parameters 

`serviceInfo`  

Dictionary that is passed back to the broadcasting app and contains information about the ongoing broadcast.

## Discussion

This method populates the serviceInfo property on RPBroadcastController to send viewing stats or messages to the broadcasting app.

## See Also

### Updating Current Broadcast Information

func updateBroadcast(URL)

Sends the current broadcast URL to the broadcast controller.

