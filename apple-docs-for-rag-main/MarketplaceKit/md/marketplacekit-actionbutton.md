

- MarketplaceKit
-  ActionButton 

Class

# ActionButton

A user-interface element that enables a person to install, update, or launch apps by tapping the element.

MarketplaceKitUIKitiOS 17.4+iPadOS 17.4+

``` source
@MainActor @objc @preconcurrency
class ActionButton
```

## Mentioned in 

Installing apps from an alternative marketplace

Supplying an install verification token

## Overview

iOS doesn’t allow an app marketplace to install apps without a person’s consent. When iOS receives a request to install an app, it validates that request came from a user interaction with this button. If instead, a marketplace calls the AppLibrary installation methods directly, the call may fail.

## Topics

### Initializers

init(action: ActionButton.Action)

### Instance Properties

let action: ActionButton.Action

var backgroundColor: UIColor?

var borderColor: UIColor

var borderWidth: CGFloat

var cornerRadius: CGFloat

var fontSize: CGFloat

var imageName: String?

var imagePlacement: ActionButton.ButtonImagePlacement

var isEnabled: Bool

var isHighlighted: Bool

var label: String

var size: CGSize

var tintColor: UIColor!

### Enumerations

enum Action

enum ButtonImagePlacement

## Relationships

### Inherits From

- UIControl

### Conforms To

- CALayerDelegate
- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
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
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### App distribution UI

struct InstallMetadata

Information about a specific app to install or update and the person who initiates it.

struct InstallConfiguration

Information that describes a requested app installation or app update.

enum InstallConfirmationResult

Options that indicate whether the installation of an app proceeds when a person interacts with an app installation button.

struct BatchInstallConfiguration

Information that describes multiple app installations or app updates.

enum BatchInstallConfirmationResult

Options that indicate whether the installation of multiple apps proceeds when a person interacts with an app installation button.

enum MarketplaceDisplayOption

The kinds of deep links that the operating system makes into your marketplace.

protocol MarketplaceSceneDelegate

A delegate that handles deep link requests into your marketplace app.

