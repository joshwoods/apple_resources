

- UIKit
-  UIMenuLeaf 

Protocol

# UIMenuLeaf

An interface for an object that represents a menu element without child elements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
protocol UIMenuLeaf : NSObjectProtocol
```

## Overview

`UIMenuLeaf` defines the behavior shared by menu elements that don’t have child elements. Don’t implement the `UIMenuLeaf` protocol in your object directly. Instead, create an appropriate object that implements this protocol, such as UIAction or UICommand.

## Topics

### Managing the appearance

var title: String

A short display title for the menu element.

**Required**

var discoverabilityTitle: String?

A long, informative title to use in the keyboard shortcut overlay.

**Required**

var image: UIImage?

An image that appears next to the menu element.

**Required**

var attributes: UIMenuElement.Attributes

The attributes that determine the style of the menu element.

**Required**

var presentationSourceItem: (any UIPopoverPresentationControllerSourceItem)?

The item you can use as an anchor for subsequent presentations.

**Required**

### Managing the selection state

var state: UIMenuElement.State

The menu element’s selection state.

**Required**

var selectedImage: UIImage?

An image that appears next to the menu element when the menu element is in the selected state.

**Required**

### Performing actions

var sender: Any?

The object on behalf of which to perform the menu element’s primary action.

**Required**

func performWithSender(Any?, target: Any?)

Performs the element’s primary action.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIAction
- UICommand
- UIKeyCommand
- UIWindowScene.ActivationAction

## See Also

### Menu elements and keyboard shortcuts

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

Adopting menus and UIActions in your user interface

Add menus to your user interface, with built-in button support and bar-button items, and create custom menu experiences.

class UIMenuElement

An object representing a menu, action, or command.

class UIAction

A menu element that performs its action in a closure.

class UICommand

A menu element that performs its action in a selector.

class UIKeyCommand

An object that specifies a key press perform on a hardware keyboard and the resulting action.

class UIDeferredMenuElement

A placeholder menu element that the system replaces with the result of the block’s completion handler.

struct Attributes

Attributes that determine the style of the menu element.

enum State

Constants that indicate the state of an action- or command-based menu element.

