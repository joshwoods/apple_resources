

- UIKit
-  Windows and screens 

API Collection

# Windows and screens

Provide a container for your view hierarchies and other content.

## Overview

Window objects act as containers for your app’s onscreen content, and screens report the characteristics of the underlying display to your app. Use Scenes to configure and manage your user interface, and review UIScreen objects to understand the device’s main screen or connected displays.

A UIWindow object provides no visible content of its own. All of the window’s visible content is provided by its root view controller, which you configure in your app’s storyboards. The window’s role is to receive events from UIKit and to forward any relevant events to the root view controller and associated views. UIKit provides an initial window for you to use, and you can create additional windows as needed.

## Topics

### Windows

class UIWindow

The backdrop for your app’s user interface and the object that dispatches events to your views.

protocol UICoordinateSpace

A set of methods for converting between different frames of reference on a screen.

### Scenes

Scenes

Manage multiple instances of your app’s UI simultaneously, and direct resources to the appropriate instance of your UI.

### Popovers

Displaying transient content in a popover

Show a temporary interface on top of your app’s content on iPad.

class UIPopoverPresentationController

An object that manages the display of content in a popover.

class UIPopoverBackgroundView

The background appearance for a popover.

protocol UIPopoverBackgroundViewMethods

A set of methods that popover background view subclasses must implement.

### Alerts

Getting the user’s attention with alerts and action sheets

Present important information to the user or prompt the user about an important choice.

class UIAlertController

An object that displays an alert message.

class UIAlertAction

An action that can be taken when the user taps a button in an alert.

### Screens

Presenting content on a connected display

Fill connected displays with additional content from your app.

class UIScreen

An object that defines the properties associated with a hardware-based display.

class UIScreenMode

A possible set of attributes that can apply to a screen object.

## See Also

### User interface

Views and controls

Present your content onscreen and define the interactions allowed with that content.

View controllers

Manage your interface using view controllers and facilitate navigation around your app’s content.

View layout

Use stack views to lay out the views of your interface automatically. Use Auto Layout when you require precise placement of your views.

Appearance customization

Add Dark Mode support to your app, customize the appearance of bars, and use appearance proxies to modify your UI.

Animation and haptics

Provide feedback to users using view-based animations and haptics.

