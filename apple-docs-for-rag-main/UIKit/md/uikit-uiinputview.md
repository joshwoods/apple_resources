

- UIKit
-  UIInputView 

Class

# UIInputView

An object that displays and manages custom input for a view when that view becomes the first responder.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIInputView
```

## Overview

The UIInputView class is designed to match the appearance of the standard system keyboard when used as an input view with a responder. When defining your own custom input views or input accessory views, you can use a UIInputView object as the root view and add any subviews you want to create your input view. The input view and its subviews receive tinting and blur effects based on the options you specify at initialization time.

Note

The effects offered by this class are applied only when the view is attached to a responder as either an input view or input accessory view. For subviews to receive style effects, they must conform to the UIAppearance protocol.

## Topics

### Initializing an input view

init(frame: CGRect, inputViewStyle: UIInputView.Style)

Initializes and returns an input view using the specified style information.

init?(coder: NSCoder)

Creates an input view from data in an unarchiver.

### Getting the input style

var inputViewStyle: UIInputView.Style

The style for the content of the view.

enum Style

Constants that indicate the appearance changes for an input view.

### Sizing the input view

var allowsSelfSizing: Bool

A Boolean value that indicates whether the input view is responsible for its own size.

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
- NSTouchBarProvider
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

### Custom keyboards

Creating a custom keyboard

Add an extension to your Xcode project to provide systemwide customized text input.

class UIInputViewController

The primary view controller for a custom keyboard app extension.

class UILexicon

A read-only array of term pairs, each in a lexicon entry object, for a custom keyboard.

class UILexiconEntry

A read-only term pair, available within a lexicon object, for a custom keyboard.

protocol UITextDocumentProxy

An object that provides textual context to a custom keyboard.

