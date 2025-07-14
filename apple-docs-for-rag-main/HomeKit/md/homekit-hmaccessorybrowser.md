

- HomeKit
-  HMAccessoryBrowser 

Class

# HMAccessoryBrowser

A network browser you can use to discover new accessories in a home.

iOS 8.0+iPadOS 8.0+visionOS 1.0+

``` source
class HMAccessoryBrowser
```

## Overview

Discovering new network accessories is an expensive operation in terms of time and power. Only start searching for new accessories when the user explicitly asks to do so, and stop searching as soon as the user has chosen the new accessories to add to their home.

Important

To enable a consistent user experience across HomeKit enabled apps, use either the addAndSetupAccessories(completionHandler:) or the addAndSetupAccessories(with:completionHandler:) method of the HMHome class instead of an accessory browser. These calls manage all the details of the accessory search process for you.

## Topics

### Discovering accessories

var discoveredAccessories: [HMAccessory]

An array of accessories discovered during a search.

func startSearchingForNewAccessories()

Starts searching for accessories not yet associated with a home.

func stopSearchingForNewAccessories()

Stops searching for new accessories.

### Tracking the addition or removal of accessories

var delegate: (any HMAccessoryBrowserDelegate)?

A delegate that receives updates on the discovered accessories.

protocol HMAccessoryBrowserDelegate

An interface used to notify an accessory browser delegate of new accessories.

### Initializers

init()

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
- Sendable

