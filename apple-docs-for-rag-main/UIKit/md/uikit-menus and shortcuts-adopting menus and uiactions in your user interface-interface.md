

- UIKit
- Menus and shortcuts
-  Adopting menus and UIActions in your user interface 

Sample Code

# Adopting menus and UIActions in your user interface

Add menus to your user interface, with built-in button support and bar-button items, and create custom menu experiences.

Download

iOS 14.0+iPadOS 14.0+Xcode 11.6+

## Overview

Note

This sample code project is associated with WWDC20 session 10052: Build with iOS Pickers, Menus and Actions.

## See Also

### Menu elements and keyboard shortcuts

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

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

protocol UIMenuLeaf

An interface for an object that represents a menu element without child elements.

