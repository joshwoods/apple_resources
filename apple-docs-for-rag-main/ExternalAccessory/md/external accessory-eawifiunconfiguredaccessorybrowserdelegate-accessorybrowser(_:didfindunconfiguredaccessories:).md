

- External Accessory
- EAWiFiUnconfiguredAccessoryBrowserDelegate
-  accessoryBrowser(\_:didFindUnconfiguredAccessories:) 

Instance Method

# accessoryBrowser(\_:didFindUnconfiguredAccessories:)

Indicates that the browser found a new unconfigured accessory that matches the filter predicate defined at the start of the search.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func accessoryBrowser(
    _ browser: EAWiFiUnconfiguredAccessoryBrowser,
    didFindUnconfiguredAccessories accessories: Set
)
```

**Required**

## Parameters 

`browser`  

The instance of EAWiFiUnconfiguredAccessoryBrowser that is generating the event.

`accessories`  

The set of EAWiFiUnconfiguredAccessory objects that have been found since the last update.

## Discussion

When a new unconfigured accessory is found, it’s added to the browser’s set of accessories, which is available in the unconfiguredAccessories property. A delegate can implement this method to present to the user the current list of unconfigured accessories. Because this method is called every time a new unconfigured accessory is found, you might use this callback as a prompt to check the list of accessories in unconfiguredAccessories.

## See Also

### Getting Updates About the Search Process

func accessoryBrowser(EAWiFiUnconfiguredAccessoryBrowser, didRemoveUnconfiguredAccessories: Set&lt;EAWiFiUnconfiguredAccessory>)

Indicates that the browser removed an unconfigured accessory from the search results.

**Required**

