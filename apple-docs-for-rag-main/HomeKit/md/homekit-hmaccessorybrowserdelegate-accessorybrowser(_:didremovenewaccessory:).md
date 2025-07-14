

- HomeKit
- HMAccessoryBrowserDelegate
-  accessoryBrowser(\_:didRemoveNewAccessory:) 

Instance Method

# accessoryBrowser(\_:didRemoveNewAccessory:)

Tells the delegate that a new accessory is no longer available in the browser.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
optional func accessoryBrowser(
    _ browser: HMAccessoryBrowser,
    didRemoveNewAccessory accessory: HMAccessory
)
```

## Parameters 

`browser`  

The browser.

`accessory`  

The accessory that is no longer available.

## Discussion

A common reason for an accessory to no longer be available is because it was added to a home, and is thus no longer a new accessory.

## See Also

### Tracking new accessories

func accessoryBrowser(HMAccessoryBrowser, didFindNewAccessory: HMAccessory)

Tells the delegate that a new accessory has been discovered.

