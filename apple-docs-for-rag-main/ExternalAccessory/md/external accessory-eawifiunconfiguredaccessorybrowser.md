

- External Accessory
-  EAWiFiUnconfiguredAccessoryBrowser 

Class

# EAWiFiUnconfiguredAccessoryBrowser

An object you use to scan for wireless accessories and configure them for use with the user’s app.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class EAWiFiUnconfiguredAccessoryBrowser
```

## Overview

The EAWiFiUnconfiguredAccessoryBrowser class gives your app access to the MFi Wireless Accessory Configuration process. You use a browser object to scan for unconfigured accessories, connect them to the user’s Wi-Fi infrastructure, and configure attributes of the accessories. An accessory is represented by an instance of EAWiFiUnconfiguredAccessory.

## Topics

### Creating the Browser Object

init(delegate: (any EAWiFiUnconfiguredAccessoryBrowserDelegate)?, queue: dispatch_queue_t?)

Creates a browser object that scans for unconfigured accessories.

### Managing Browser Interactions

var delegate: (any EAWiFiUnconfiguredAccessoryBrowserDelegate)?

The object that acts as the delegate of the browser and receives browser events.

protocol EAWiFiUnconfiguredAccessoryBrowserDelegate

A protocol you use to manage the search and configuration processes for an unconfigured accessory browser.

### Finding and Configuring Accessories

func configureAccessory(EAWiFiUnconfiguredAccessory, withConfigurationUIOn: UIViewController)

Begins the configuration process for the specified accessory.

func startSearchingForUnconfiguredAccessories(matching: NSPredicate?)

Starts the search for unconfigured accessories that match the specified predicate.

func stopSearchingForUnconfiguredAccessories()

Stops the search for unconfigured accessories.

var unconfiguredAccessories: Set&lt;EAWiFiUnconfiguredAccessory>

The set of unconfigured accessories that have been discovered.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Wi-Fi Accessory Configuration

Wireless Accessory Configuration Entitlement

A Boolean value that indicates whether your app may configure MFi Wi-Fi accessories.

class EAWiFiUnconfiguredAccessory

An object that provides information about an unconfigured MFi Wireless Accessory Configuration accessory.

