

- StoreKit
-  SKStoreProductViewController 

Class

# SKStoreProductViewController

A view controller that provides a page where customers can purchase media from the App Store.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+macOS 11.0+

``` source
@MainActor
class SKStoreProductViewController
```

## Mentioned in 

Signing and providing ads

Receiving ad attributions and postbacks

## Overview

To display a store for customers to purchase media from the App Store, follow these steps:

1.  Create an `SKStoreProductViewController` object and set its delegate.

2.  Indicate a specific product to sell by passing its iTunes item identifier to the loadProduct(withParameters:completionBlock:) method.

3.  Present the view controller modally from another view controller in your app. Your delegate dismisses the view controller when the customer completes the purchase.

Present the `SKStoreProductViewController` object immediately when someone triggers an interaction, such as tapping a Buy button. Load the product information before presenting the view controller to ensure a seamless user experience.

This class ignores modalPresentationStyle settings, and those settings have no impact on the sheet’s presentation.

To recommend another app without displaying a full product page, and to recommend an App Clip’s corresponding app from within the App Clip, use SKOverlay.

Note

In a compatible iPad or iPhone app running in visionOS, this method displays a minimal sheet to enable an app purchase or to launch the App Store for more information. For an in-line experience that’s consistent across platforms, use SKOverlay instead.

### Prevent exceptions

The `SKStoreProductViewController` class doesn’t support subclassing or embedding, and must be used as-is.

Important

If you compile with the iOS 13 SDK, attempting to instantiate a subclass of `SKStoreProductViewController` results in a runtime exception.

This class throws the following runtime exceptions:

SKUnsupportedClassException  
Occurs if the app attempts to instantiate a subclass of `SKStoreProductViewController`.

SKUnsupportedPresentationException  
Occurs if the app attempts to use an unsupported presentation mode for `SKStoreProductViewController`, such as embedding it as a subview controller or attempting to use it in a popover.

## Topics

### Setting a delegate

var delegate: (any SKStoreProductViewControllerDelegate)?

The store view controller’s delegate.

protocol SKStoreProductViewControllerDelegate

A protocol to call when the customer dismisses the store screen.

### Loading a new product screen

Offering media for sale in your app

Allow users to purchase media in the App Store from within your app.

func loadProduct(withParameters: [String : Any], completionBlock: ((Bool, (any Error)?) -> Void)?)

Loads a new product screen to display.

func loadProduct(withParameters: [String : Any], impression: SKAdImpression, completionBlock: ((Bool, (any Error)?) -> Void)?)

func loadProduct(parameters: [String : Any], impression: AppImpression) async throws

func loadProduct(parameters: [String : Any], impression: AppImpression, reengagementURL: URL) async throws

Product Dictionary Keys

Keys for identifying products and the tokens for affiliates and campaigns.

## Relationships

### Inherits From

- NSViewController
- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSEditor
- NSExtensionRequestHandling
- NSObjectProtocol
- NSSeguePerforming
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable
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

### Recommendations

Offering media for sale in your app

Allow users to purchase media in the App Store from within your app.

class SKOverlay

A class that displays an overlay you can use to recommend another app or an App Clip’s corresponding full app.

