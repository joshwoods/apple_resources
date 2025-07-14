

- HomeKit
- HMAccessoryBrowser
-  discoveredAccessories 

Instance Property

# discoveredAccessories

An array of accessories discovered during a search.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
var discoveredAccessories: [HMAccessory] { get }
```

## Discussion

When you start a new search by calling the startSearchingForNewAccessories() method, HomeKit clears the discoveredAccessories array. It then modifies the array as it discovers new accessories until you end the search by calling the stopSearchingForNewAccessories() method.

## See Also

### Discovering accessories

func startSearchingForNewAccessories()

Starts searching for accessories not yet associated with a home.

func stopSearchingForNewAccessories()

Stops searching for new accessories.

