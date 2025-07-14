

- External Accessory
- EAWiFiUnconfiguredAccessoryBrowserDelegate
-  accessoryBrowser(\_:didRemoveUnconfiguredAccessories:) 

Instance Method

# accessoryBrowser(\_:didRemoveUnconfiguredAccessories:)

Indicates that the browser removed an unconfigured accessory from the search results.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func accessoryBrowser(
    _ browser: EAWiFiUnconfiguredAccessoryBrowser,
    didRemoveUnconfiguredAccessories accessories: Set
)
```

**Required**

## Parameters 

`browser`  

The instance of EAWiFiUnconfiguredAccessoryBrowser that is generating the event.

`accessories`  

The set of EAWiFiUnconfiguredAccessory objects that have been removed from the scan results since the last update. The browser removes only accessories that match the filter predicate you specified at the start of the search.

## Discussion

This method is called when the browser removes an accessory from the primary list of unconfigured accessories represented in its unconfiguredAccessories property. A delegate can implement this method to present to the user the current list of unconfigured accessories. Because this method is called every time an unconfigured accessory is removed from the list, you might use this callback as a prompt to check the list of accessories in unconfiguredAccessories.

## See Also

### Getting Updates About the Search Process

func accessoryBrowser(EAWiFiUnconfiguredAccessoryBrowser, didFindUnconfiguredAccessories: Set&lt;EAWiFiUnconfiguredAccessory>)

Indicates that the browser found a new unconfigured accessory that matches the filter predicate defined at the start of the search.

**Required**

