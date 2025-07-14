

- External Accessory
- EAWiFiUnconfiguredAccessoryBrowserDelegate
-  accessoryBrowser(\_:didUpdate:) 

Instance Method

# accessoryBrowser(\_:didUpdate:)

Indicates that the browser’s state has changed.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func accessoryBrowser(
    _ browser: EAWiFiUnconfiguredAccessoryBrowser,
    didUpdate state: EAWiFiUnconfiguredAccessoryBrowserState
)
```

**Required**

## Parameters 

`browser`  

The instance of EAWiFiUnconfiguredAccessoryBrowser that is generating the event.

`state`  

The current state of the browser. See EAWiFiUnconfiguredAccessoryBrowserState for possible values.

## Discussion

When the browser state changes, the delegate typically provides feedback to users. For example, the delegate might show whether the scan is currently active or inactive, or it might indicate that Wi-Fi is unavailable if a user starts a scan while the device is in airplane mode.

## See Also

### Getting Updates About Browser State

enum EAWiFiUnconfiguredAccessoryBrowserState

The possible states of an accessory browser.

