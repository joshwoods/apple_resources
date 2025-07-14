

- External Accessory
- EAWiFiUnconfiguredAccessoryBrowser
-  stopSearchingForUnconfiguredAccessories() 

Instance Method

# stopSearchingForUnconfiguredAccessories()

Stops the search for unconfigured accessories.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func stopSearchingForUnconfiguredAccessories()
```

## See Also

### Finding and Configuring Accessories

func configureAccessory(EAWiFiUnconfiguredAccessory, withConfigurationUIOn: UIViewController)

Begins the configuration process for the specified accessory.

func startSearchingForUnconfiguredAccessories(matching: NSPredicate?)

Starts the search for unconfigured accessories that match the specified predicate.

var unconfiguredAccessories: Set&lt;EAWiFiUnconfiguredAccessory>

The set of unconfigured accessories that have been discovered.

