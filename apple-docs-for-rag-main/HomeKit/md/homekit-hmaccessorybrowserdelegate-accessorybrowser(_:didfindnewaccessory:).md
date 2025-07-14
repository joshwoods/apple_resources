

- HomeKit
- HMAccessoryBrowserDelegate
-  accessoryBrowser(\_:didFindNewAccessory:) 

Instance Method

# accessoryBrowser(\_:didFindNewAccessory:)

Tells the delegate that a new accessory has been discovered.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
optional func accessoryBrowser(
    _ browser: HMAccessoryBrowser,
    didFindNewAccessory accessory: HMAccessory
)
```

## Parameters 

`browser`  

The browser that discovered the new accessory.

`accessory`  

The new accessory.

## See Also

### Tracking new accessories

func accessoryBrowser(HMAccessoryBrowser, didRemoveNewAccessory: HMAccessory)

Tells the delegate that a new accessory is no longer available in the browser.

