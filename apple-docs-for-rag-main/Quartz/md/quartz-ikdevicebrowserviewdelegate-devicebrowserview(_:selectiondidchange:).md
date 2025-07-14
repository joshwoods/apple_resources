

- Quartz
- IKDeviceBrowserViewDelegate
-  deviceBrowserView(\_:selectionDidChange:) 

Instance Method

# deviceBrowserView(\_:selectionDidChange:)

Sent to the delegate when the selection changes in the browser view.

macOS 10.6+

``` source
func deviceBrowserView(
    _ deviceBrowserView: IKDeviceBrowserView!,
    selectionDidChange device: ICDevice!
)
```

**Required**

## Parameters 

`deviceBrowserView`  

The object that sent the message.

`device`  

The newly selected device.

