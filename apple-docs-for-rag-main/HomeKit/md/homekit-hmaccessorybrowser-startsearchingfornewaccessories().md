

- HomeKit
- HMAccessoryBrowser
-  startSearchingForNewAccessories() 

Instance Method

# startSearchingForNewAccessories()

Starts searching for accessories not yet associated with a home.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
func startSearchingForNewAccessories()
```

## Discussion

HomeKit notifies your accessory browser delegate by calling the accessoryBrowser(_:didFindNewAccessory:) and accessoryBrowser(_:didRemoveNewAccessory:) methods when it detects accessories being added or removed, respectively.

When you start a search, HomeKit clears the discoveredAccessories array of content from the previous search.

## See Also

### Discovering accessories

var discoveredAccessories: [HMAccessory]

An array of accessories discovered during a search.

func stopSearchingForNewAccessories()

Stops searching for new accessories.

