

- TVMLKit
-  TVBrowserViewController 

Class

# TVBrowserViewController

A view controller that presents content in a browsable, full-screen format.

tvOS 13.0+

``` source
@MainActor
class TVBrowserViewController
```

## Overview

Use this class to create a full-screen layout that supports full-screen browsing. This layout includes a built-in parallax effect that is triggered during the transition between cells.

## Topics

### Initializing the Browser View Controller

convenience init?(viewElement: TVViewElement)

Create a full-screen browser from a specified view element.

### Providing the Browser’s Data

var dataSource: (any TVBrowserViewControllerDataSource)?

The object that provides data to the full-screen browser.

protocol TVBrowserViewControllerDataSource

Methods adopted by the object you use to represent the browser view.

### Managing Interactions with the Browser

var delegate: (any TVBrowserViewControllerDelegate)?

The object that acts as the delegate and handles callbacks for the browser view.

protocol TVBrowserViewControllerDelegate

Methods for detecting events and performing actions on the browser view.

### Modifying the Browser Appearance

var cornerRadius: CGFloat

The corner radius, in points, of each full-screen browser item.

var interitemSpacing: CGFloat

The spacing between full-screen browser items.

var maskInset: UIEdgeInsets

The amount by which the content of the cell is inset.

### Accessing Browser Elements

var centeredViewElement: TVViewElement

The full screen browser item that is currently centered on the screen.

var viewElement: TVViewElement

The view element that the full screen browser is constructed from.

### Managing Browser Transitions

class TVBrowserTransitionAnimator

An object that provides animations to and from the full screen browser.

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
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Views and View Controllers

class TVViewElement

A representation of a read-only DOM node.

Deprecated

protocol TVInterfaceCreating

A protocol that defines methods used to create views and view controllers.

Deprecated

class TVInterfaceFactory

A factory for the creation of views and view controllers.

Deprecated

class TVDocumentViewController

A view controller that represents a TVMLKit document.

Deprecated

