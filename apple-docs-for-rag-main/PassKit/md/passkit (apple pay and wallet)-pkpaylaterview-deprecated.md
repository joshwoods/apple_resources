

- PassKit (Apple Pay and Wallet)
-  PKPayLaterView Deprecated

Class

# PKPayLaterView

A view that displays the Apple Pay Later visual merchandising widget.

iOS 17.0+iPadOS 17.0+visionOS 1.0+

``` source
@MainActor
class PKPayLaterView
```

Deprecated

Apple Pay Later is deprecated.

## Overview

Use this view to display a widget that allows people to learn more about the Apple Pay Later feature.

## Topics

### Creating the widget

convenience init(amount: Decimal, currency: Locale.Currency)

Creates a new Apple Pay Later visual merchandising widget view with the shopping cart amount and currency you specify.

### Accessing information about the transaction

var amount: Decimal

The decimal value that represents the amount of the customer’s shopping cart or item pricing.

var currency: Locale.Currency

The ISO-4217 currency code for the country or region of the merchant’s principle place of business.

### Responding to changes in the view’s height

var delegate: any PKPayLaterViewDelegate

A delegate object that receives messages about the changes to the Apple Pay Later view.

protocol PKPayLaterViewDelegate

Methods the framework calls when the Apple Pay Later view’s size changes.

### Setting the user action

var action: PKPayLaterAction

The information style that the Apple Pay Later view presents.

enum PKPayLaterAction

Values you use to set the Apple Pay Later action.

### Styling the view

var displayStyle: PKPayLaterDisplayStyle

The style to use when presenting the Apple Pay Later visual merchandising widget view.

enum PKPayLaterDisplayStyle

Values you use to style an Apple Pay Later visual merchandising widget.

### Validating transactions

enum PKPayLater

Functions for validating information the framework displays in an Apple Pay Later visual merchandising widget.

## Relationships

### Inherits From

- UIView

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable
- UIAccessibilityIdentification
- UIActivityItemsConfigurationProviding
- UIAppearance
- UIAppearanceContainer
- UICoordinateSpace
- UIDynamicItem
- UIFocusEnvironment
- UIFocusItem
- UIFocusItemContainer
- UILargeContentViewerItem
- UIPasteConfigurationSupporting
- UIPopoverPresentationControllerSourceItem
- UIResponderStandardEditActions
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Deprecated

struct PayLaterView

A view that displays the Apple Pay Later visual merchandising widget.

Deprecated

