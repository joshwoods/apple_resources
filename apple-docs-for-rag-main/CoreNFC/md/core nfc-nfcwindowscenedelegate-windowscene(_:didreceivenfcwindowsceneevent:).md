

- Core NFC
- NFCWindowSceneDelegate
-  windowScene(\_:didReceiveNFCWindowSceneEvent:) 

Instance Method

# windowScene(\_:didReceiveNFCWindowSceneEvent:)

Informs your app that the system has received an NFC-related event.

CoreNFCUIKitiOS 17.4+iPadOS 17.4+Mac Catalyst

``` source
func windowScene(
    _ windowScene: UIWindowScene,
    didReceiveNFCWindowSceneEvent event: NFCWindowSceneEvent
)
```

**Required**

## Parameters 

`windowScene`  

A scene in your app that handles the event.

`event`  

The NFC-related event that triggered the delegate callback.

## See Also

### Handling events

enum NFCWindowSceneEvent

An NFC-related event that your app uses to update its user interface.

