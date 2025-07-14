

- External Accessory
-  EAWiFiUnconfiguredAccessoryBrowserDelegate 

Protocol

# EAWiFiUnconfiguredAccessoryBrowserDelegate

A protocol you use to manage the search and configuration processes for an unconfigured accessory browser.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
protocol EAWiFiUnconfiguredAccessoryBrowserDelegate : NSObjectProtocol
```

## Topics

### Getting Updates About Browser State

func accessoryBrowser(EAWiFiUnconfiguredAccessoryBrowser, didUpdate: EAWiFiUnconfiguredAccessoryBrowserState)

Indicates that the browser’s state has changed.

**Required**

enum EAWiFiUnconfiguredAccessoryBrowserState

The possible states of an accessory browser.

### Getting Updates About the Configuration Process

func accessoryBrowser(EAWiFiUnconfiguredAccessoryBrowser, didFinishConfiguringAccessory: EAWiFiUnconfiguredAccessory, with: EAWiFiUnconfiguredAccessoryConfigurationStatus)

Indicates that the browser has completed configuring the specified accessory.

**Required**

enum EAWiFiUnconfiguredAccessoryConfigurationStatus

Values that represent the state of the configuration process for an EAWiFiUnconfiguredAccessory object.

### Getting Updates About the Search Process

func accessoryBrowser(EAWiFiUnconfiguredAccessoryBrowser, didFindUnconfiguredAccessories: Set&lt;EAWiFiUnconfiguredAccessory>)

Indicates that the browser found a new unconfigured accessory that matches the filter predicate defined at the start of the search.

**Required**

func accessoryBrowser(EAWiFiUnconfiguredAccessoryBrowser, didRemoveUnconfiguredAccessories: Set&lt;EAWiFiUnconfiguredAccessory>)

Indicates that the browser removed an unconfigured accessory from the search results.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing Browser Interactions

var delegate: (any EAWiFiUnconfiguredAccessoryBrowserDelegate)?

The object that acts as the delegate of the browser and receives browser events.

