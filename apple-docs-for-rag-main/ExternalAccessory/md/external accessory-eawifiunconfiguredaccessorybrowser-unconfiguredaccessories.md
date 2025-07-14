

- External Accessory
- EAWiFiUnconfiguredAccessoryBrowser
-  unconfiguredAccessories 

Instance Property

# unconfiguredAccessories

The set of unconfigured accessories that have been discovered.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
var unconfiguredAccessories: Set { get }
```

## Discussion

The set of accessories in this property represents a snapshot that includes only those objects that match the filter predicate defined when starting the search. You can think of this property as representing the primary list of unconfigured accessories that have been found. Note that the accessoryBrowser(_:didFindUnconfiguredAccessories:) delegate method is called when accessories are added to this list; similarly, accessoryBrowser(_:didRemoveUnconfiguredAccessories:) is called when accessories are removed from this list.

## See Also

### Finding and Configuring Accessories

func configureAccessory(EAWiFiUnconfiguredAccessory, withConfigurationUIOn: UIViewController)

Begins the configuration process for the specified accessory.

func startSearchingForUnconfiguredAccessories(matching: NSPredicate?)

Starts the search for unconfigured accessories that match the specified predicate.

func stopSearchingForUnconfiguredAccessories()

Stops the search for unconfigured accessories.

