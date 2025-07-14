

- AppKit
-  NSSeguePerforming 

Protocol

# NSSeguePerforming

A set of methods that support the mediation of a custom segue.

macOS

``` source
protocol NSSeguePerforming : NSObjectProtocol
```

## Overview

When you subclass NSStoryboardSegue to express a custom transition or containment relationship between storyboard scenes, you might also want to provide code that prepares the destination/contained view or window controller object. Put this code in an override of the prepare(for:sender:) method.

To conditionally disallow the performance of a segue, override the shouldPerformSegue(withIdentifier:sender:) method, returning false.If you need to programmatically trigger a segue that cannot be expressed in a storyboard file, such as a transition between scenes in different storyboards, use the performSegue(withIdentifier:sender:) method in this protocol.

## Topics

### Working with Storyboard Segues

func performSegue(withIdentifier: NSStoryboardSegue.Identifier, sender: Any?)

Performs the specified segue.

func prepare(for: NSStoryboardSegue, sender: Any?)

Called when a segue is about to be performed.

func shouldPerformSegue(withIdentifier: NSStoryboardSegue.Identifier, sender: Any?) -> Bool

Called immediately prior to the performance of a storyboard segue.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSCollectionViewItem
- NSPageController
- NSSplitViewController
- NSTabViewController
- NSTitlebarAccessoryViewController
- NSViewController
- NSWindowController

## See Also

### Storyboard

class NSStoryboard

An encapsulation of the design-time view controller and window controller graph represented in an Interface Builder storyboard resource file.

class NSStoryboardSegue

A transition or containment relationship between two scenes in a storyboard.

