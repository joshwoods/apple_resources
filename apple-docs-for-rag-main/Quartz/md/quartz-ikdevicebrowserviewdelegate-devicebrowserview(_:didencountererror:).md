

- Quartz
- IKDeviceBrowserViewDelegate
-  deviceBrowserView(\_:didEncounterError:) 

Instance Method

# deviceBrowserView(\_:didEncounterError:)

Invoked when the device browser encounters an error.

macOS 10.6+

``` source
optional func deviceBrowserView(
    _ deviceBrowserView: IKDeviceBrowserView!,
    didEncounterError error: (any Error)!
)
```

## Parameters 

`deviceBrowserView`  

The object that sent the message.

`error`  

The error the device browser encountered.

## Discussion

The user should handle the error in some fashion, for example, presenting an error panel to the user.

