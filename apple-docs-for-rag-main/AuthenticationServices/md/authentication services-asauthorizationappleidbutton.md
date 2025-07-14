

- Authentication Services
-  ASAuthorizationAppleIDButton 

Class

# ASAuthorizationAppleIDButton

A control you add to your interface that enables users to initiate the Sign In with Apple flow.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class ASAuthorizationAppleIDButton
```

## Overview

Choose one of the built-in button styles and types, and change the corner radius of the button by setting the cornerRadius property, but don’t otherwise modify the style of the button. Don’t use an Apple ID authorization button for any purpose other than to initiate the Sign In with Apple flow.

After the user taps the button, create a request using the provider, and then use an instance of ASAuthorizationController to execute the request.

## Topics

### Initializers

init(authorizationButtonType: ASAuthorizationAppleIDButton.ButtonType, authorizationButtonStyle: ASAuthorizationAppleIDButton.Style)

Creates a new Sign In with Apple authorization button with the given type and style.

convenience init(type: ASAuthorizationAppleIDButton.ButtonType, style: ASAuthorizationAppleIDButton.Style)

Creates a new Sign In with Apple authorization button with the given type and style.

### Styling the Button

var cornerRadius: CGFloat

The radius, in points, for the rounded corners on the Apple ID sign-in button.

enum Style

A style for the authorization button.

enum ButtonType

A type for the authorization button.

## Relationships

### Inherits From

- NSControl
- UIControl

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
- NSUserInterfaceItemIdentification
- Sendable
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

### Offering Sign In with Apple

class WKInterfaceAuthorizationAppleIDButton

A button that you can use to trigger a Sign in with Apple request.

