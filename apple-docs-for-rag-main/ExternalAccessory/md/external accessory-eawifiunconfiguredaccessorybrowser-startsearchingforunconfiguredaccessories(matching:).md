

- External Accessory
- EAWiFiUnconfiguredAccessoryBrowser
-  startSearchingForUnconfiguredAccessories(matching:) 

Instance Method

# startSearchingForUnconfiguredAccessories(matching:)

Starts the search for unconfigured accessories that match the specified predicate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func startSearchingForUnconfiguredAccessories(matching predicate: NSPredicate?)
```

## Parameters 

`predicate`  

The desired filter for unconfigured accessory results conforming to the EAWiFiUnconfiguredAccessoryBrowserDelegate protocol.

## Discussion

This method starts a Wi-Fi scan for unconfigured accessories. Note that searching is a power and resource intensive process and must only be used when actively searching for accessories. As soon as the desired accessories have been located, you should immediately stop a search.

## See Also

### Finding and Configuring Accessories

func configureAccessory(EAWiFiUnconfiguredAccessory, withConfigurationUIOn: UIViewController)

Begins the configuration process for the specified accessory.

func stopSearchingForUnconfiguredAccessories()

Stops the search for unconfigured accessories.

var unconfiguredAccessories: Set&lt;EAWiFiUnconfiguredAccessory>

The set of unconfigured accessories that have been discovered.

