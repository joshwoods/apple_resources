

- HomeKit
-  HMAccessoryBrowserDelegate 

Protocol

# HMAccessoryBrowserDelegate

An interface used to notify an accessory browser delegate of new accessories.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
protocol HMAccessoryBrowserDelegate : NSObjectProtocol
```

## Overview

Important

To enable a consistent user experience across HomeKit enabled apps, use either the addAndSetupAccessories(completionHandler:) or the addAndSetupAccessories(with:completionHandler:) method of the HMHome class instead of an accessory browser. These calls manage all the details of the accessory search process for you.

## Topics

### Tracking new accessories

func accessoryBrowser(HMAccessoryBrowser, didFindNewAccessory: HMAccessory)

Tells the delegate that a new accessory has been discovered.

func accessoryBrowser(HMAccessoryBrowser, didRemoveNewAccessory: HMAccessory)

Tells the delegate that a new accessory is no longer available in the browser.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Tracking the addition or removal of accessories

var delegate: (any HMAccessoryBrowserDelegate)?

A delegate that receives updates on the discovered accessories.

