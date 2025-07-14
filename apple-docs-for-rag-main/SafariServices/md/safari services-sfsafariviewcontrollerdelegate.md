

- Safari Services
-  SFSafariViewControllerDelegate 

Protocol

# SFSafariViewControllerDelegate

A protocol used to implement custom event handling for a Safari view controller.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+

``` source
protocol SFSafariViewControllerDelegate : NSObjectProtocol
```

## Overview

For more information about the `SFSafariViewController` class, see SFSafariViewController.

## Topics

### Working with the View Controller

func safariViewController(SFSafariViewController, didCompleteInitialLoad: Bool)

Tells the delegate that the initial URL load completed.

func safariViewController(SFSafariViewController, activityItemsFor: URL, title: String?) -> [UIActivity]

Tells the delegate that the user tapped an Action button.

func safariViewControllerDidFinish(SFSafariViewController)

Tells the delegate that the user dismissed the view.

func safariViewController(SFSafariViewController, excludedActivityTypesFor: URL, title: String?) -> [UIActivity.ActivityType]

### Instance Methods

func safariViewController(SFSafariViewController, initialLoadDidRedirectTo: URL)

func safariViewControllerWillOpenInBrowser(SFSafariViewController)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Responding to View Controller Interaction

var delegate: (any SFSafariViewControllerDelegate)?

An object that provides behavior for the Safari view controller’s Done and Action buttons.

