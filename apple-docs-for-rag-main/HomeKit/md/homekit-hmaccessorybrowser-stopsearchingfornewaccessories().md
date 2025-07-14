

- HomeKit
- HMAccessoryBrowser
-  stopSearchingForNewAccessories() 

Instance Method

# stopSearchingForNewAccessories()

Stops searching for new accessories.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
func stopSearchingForNewAccessories()
```

## Discussion

After you call this method, HomeKit stops sending updates to your browser delegate. Scanning may continue for system reasons or if other delegates are still active, but the discoveredAccessories array remains unchanged after you stop the search until your app calls the startSearchingForNewAccessories() method again.

## See Also

### Discovering accessories

var discoveredAccessories: [HMAccessory]

An array of accessories discovered during a search.

func startSearchingForNewAccessories()

Starts searching for accessories not yet associated with a home.

