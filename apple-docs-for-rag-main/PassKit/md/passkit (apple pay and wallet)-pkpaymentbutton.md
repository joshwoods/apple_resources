

- PassKit (Apple Pay and Wallet)
-  PKPaymentButton 

Class

# PKPaymentButton

An object that displays a button either to trigger payments through Apple Pay or to prompt the user to set up a card.

iOS 8.3+iPadOS 8.3+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
@MainActor
class PKPaymentButton
```

## Overview

After creating a PKPaymentButton object, you choose the type and style of button, and the system provides a control with the correct content and appearance. See the Human Interface Guidelines > Apple Pay for more information.

To trigger a payment through Apple Pay in a WatchKit app, use WKInterfacePaymentButton instead.

## Topics

### Creating payment buttons

init(paymentButtonType: PKPaymentButtonType, paymentButtonStyle: PKPaymentButtonStyle)

Creates a new payment button with the specified type and style.

### Configuring the appearance

enum PKPaymentButtonType

The Apple Pay button types you can display to initiate Apple Pay transactions.

enum PKPaymentButtonStyle

A type that indicates the available appearances for an Apple Pay button.

var cornerRadius: CGFloat

The radius, in points, for the rounded corners on the button.

## Relationships

### Inherits From

- NSButton
- UIButton

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityButton
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceCompression
- NSUserInterfaceItemIdentification
- NSUserInterfaceValidations
- Sendable
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

### Related Documentation

iOS Human Interface Guidelines

### Apple Pay buttons

struct PayWithApplePayButton

struct PayWithApplePayButtonLabel

struct PayWithApplePayButtonStyle

