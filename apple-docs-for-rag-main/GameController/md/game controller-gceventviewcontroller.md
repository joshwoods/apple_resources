

- Game Controller
-  GCEventViewController 

Class

# GCEventViewController

A view controller that delivers input either from the responder chain to views, or from game controllers to profiles.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class GCEventViewController
```

## Mentioned in 

Adding touch controls to games that support game controllers in iOS

## Overview

On systems, such as tvOS, where the player uses the game controller to both navigate the system interface and play your game, use a GCEventViewController object as the root view controller to selectively receive input directly from the game controller. You can’t simultaneously process input through the responder chain and Game Controller input elements.

By default the system delivers input events to your app using the responder chain. To get the input values through the game controller objects, set a GCEventViewController object as the root view controller. The view controller delivers the input for its views and their subviews to the game controller’s profile. To switch back to the responder chain, set the view controller’s controllerUserInteractionEnabled property to true.

## Topics

### Delivering game controller inputs

var controllerUserInteractionEnabled: Bool

A Boolean value that indicates whether the system delivers game controller input to profile objects or to views using the responder chain.

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

