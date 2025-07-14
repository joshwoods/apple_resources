

- UIKit
-  UIFocusGuide 

Class

# UIFocusGuide

An object that exposes nonview areas as focusable.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class UIFocusGuide
```

## Mentioned in 

Creating custom navigation interactions

Adding user-focusable elements to a tvOS app

## Overview

As a subclass of UILayoutGuide, a focus guide is not a view and does not define a new view or participate in the view hierarchy at all, except as an Auto Layout guide. Unlike UILayoutGuide, UIFocusGuide represents an invisible, focusable region that can redirect focus movement to other views. The `UIFocus.h` header file, including its related classes and its protocol, creates a single high-level software interface for controlling focus in apps that use focus-based input. This programming interface also helps to control focus behavior on the screen.

## Topics

### Enabling focus

var isEnabled: Bool

A Boolean value that indicates whether the guide is focusable.

var preferredFocusEnvironments: [any UIFocusEnvironment]!

An array of focus environments to which the guide directs focus, ordered by priority.

var preferredFocusedView: UIView?

The view that the focus will be redirected to if this guide is focused.

Deprecated

## Relationships

### Inherits From

- UILayoutGuide

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- UIPopoverPresentationControllerSourceItem

## See Also

### Focus guides

Creating custom navigation interactions

Build nonstandard navigation interactions that move focus to the desired location.

