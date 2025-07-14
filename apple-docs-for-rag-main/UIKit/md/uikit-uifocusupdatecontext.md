

- UIKit
-  UIFocusUpdateContext 

Class

# UIFocusUpdateContext

An object that provides information relevant to a specific focus update from one view to another.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class UIFocusUpdateContext
```

## Overview

Focus update context objects are ephemeral and are usually discarded after the update is finished. The `UIFocus` APIs create a single high-level software interface for controlling focus in apps that use focus-based input.

## Topics

### Locating focus direction

var previouslyFocusedView: UIView?

The view that was focused before the focus update.

var nextFocusedView: UIView?

The view that takes the focus after the focus update.

var focusHeading: UIFocusHeading

The heading in which the focus update is occurring.

struct UIFocusHeading

The general type of an event.

### Getting related focus items

var previouslyFocusedItem: (any UIFocusItem)?

The item that was focused before the update.

var nextFocusedItem: (any UIFocusItem)?

The item to be focused after the update.

### Responding to focus-related keys and notifications

class let didUpdateNotification: NSNotification.Name

The focus for the UI has been updated.

class let movementDidFailNotification: NSNotification.Name

The focus failed to move to another item.

class let animationCoordinatorUserInfoKey: String

Updates the animation coordinator.

class let focusUpdateContextUserInfoKey: String

Updates the context key.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UICollectionViewFocusUpdateContext
- UITableViewFocusUpdateContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Focus interactions

Navigating an app’s user interface using a keyboard

Navigate between user interface elements using a keyboard and focusable UI elements in iPad apps and apps built with Mac Catalyst.

About focus interactions for Apple TV

Design and implement intuitive control schemes for menus and interactive user interface layouts.

Adding user-focusable elements to a tvOS app

Create intuitive and easily manipulated user-interactive controls for your tvOS app.

protocol UIFocusEnvironment

A set of methods that define the focus behavior for a branch of the view hierarchy.

class UIFocusSystem

Queries and reevaluates the currently focused item.

protocol UIFocusItem

An object that can become focused.

class UIFocusMovementHint

Provides movement hint information for the focused item.

protocol UIFocusItemContainer

The container responsible for providing geometric context to focus items within a given focus environment.

protocol UIFocusItemScrollableContainer

A type of focus item container that supports automatic scrolling of focusable content.

struct UIFocusGroupPriority

The importance of an item within a focus group, used by the focus system to determine the group’s primary item.

