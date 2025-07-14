

- AppKit
-  NSViewControllerPresentationAnimator 

Protocol

# NSViewControllerPresentationAnimator

A set of methods that let you define animations to play when transitioning between two view controllers.

macOS

``` source
protocol NSViewControllerPresentationAnimator : NSObjectProtocol
```

## Overview

Implement this protocol only if you want to provide custom animations. You might find what you need in the NSViewController.TransitionOptions enumeration, which provides many predefined animations.

A class that adopts this protocol is responsible for both presenting and dismissing a view controller.

## Topics

### Animating Presentation and Dismissal of View Controllers

func animatePresentation(of: NSViewController, from: NSViewController)

Called when the specified view controller is about to be presented.

**Required**

func animateDismissal(of: NSViewController, from: NSViewController)

Called when a previously-presented view controller is about to be dismissed.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

