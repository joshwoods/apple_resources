

- StoreKit
-  SKCloudServiceSetupViewController Deprecated

Class

# SKCloudServiceSetupViewController

A view controller that helps people perform setup for a cloud service, like an Apple Music subscription.

iOS 10.1–18.0DeprecatediPadOS 10.1–18.0DeprecatedMac Catalyst 13.1–18.0Deprecated

``` source
@MainActor
class SKCloudServiceSetupViewController
```

Deprecated

Use musicSubscriptionOffer(isPresented:options:onLoadCompletion:) instead.

## Mentioned in 

Offering Apple Music Subscription in Your App

Determining a person’s Apple Music capabilities

## Overview

Use the view that this view controller presents to allow customers to set up cloud services that are associated with their iTunes Store account, like an Apple Music subscription.

To enable the Apple Music subscriber setup flow in particular, you first request the current set of capabilities from SKCloudServiceController. Then, present the setup view controller only when the musicCatalogSubscriptionEligible capability is enabled and the musicCatalogPlayback capability is disabled.

For information about other capabilities that you can enable by using this view controller, see SKCloudServiceCapability.

## Topics

### Setting a delegate

var delegate: (any SKCloudServiceSetupViewControllerDelegate)?

The cloud service view controller’s delegate.

protocol SKCloudServiceSetupViewControllerDelegate

A protocol that defines the methods a cloud service setup view controller can use to get the status of the view, including when it is dismissed.

### Loading the setup view

Offering Apple Music Subscription in Your App

Allow eligible customers to subscribe to Apple Music.

struct SKCloudServiceSetupOptionsKey

Keys to specify the types of setup options for a cloud service.

func load(options: [SKCloudServiceSetupOptionsKey : Any], completionHandler: ((Bool, (any Error)?) -> Void)?)

Loads the cloud service setup view with the specified options.

class SKArcadeService

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Deprecated

class SKCloudServiceController

An object that determines the current capabilities of a person’s Music library.

Deprecated

