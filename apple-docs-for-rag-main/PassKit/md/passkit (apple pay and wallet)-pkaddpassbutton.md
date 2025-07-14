

- PassKit (Apple Pay and Wallet)
-  PKAddPassButton 

Class

# PKAddPassButton

Provides a button that enables users to add passes to Wallet.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class PKAddPassButton
```

## Overview

When you use the PKAddPassButton class to create a button, you choose the button’s style, and the system provides a control with the correct appearance.

## Topics

### Creating add pass buttons

init(addPassButtonStyle: PKAddPassButtonStyle)

Initializes a new Add Pass button.

### Accessing the button’s style

var addPassButtonStyle: PKAddPassButtonStyle

A constant representing the button’s style.

### Button styles

enum PKAddPassButtonStyle

The appearance of the buttons that can be created using the addPassButtonWithStyle: method.

## Relationships

### Inherits From

- UIButton

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSTouchBarProvider
- UIAccessibilityContentSizeCategoryImageAdjusting
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UIContextMenuInteractionDelegate
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UISpringLoadedInteractionSupporting
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Common objects

class PKObject

An opaque type that acts as the superclass for the pass object.

class PKLabeledValue

An object that can represent a detail about a payment card or other item.

struct AddPassToWalletButton

struct AddPassToWalletButtonFilter

struct AddPassToWalletButtonResponse

struct AddPassToWalletButtonStyle

