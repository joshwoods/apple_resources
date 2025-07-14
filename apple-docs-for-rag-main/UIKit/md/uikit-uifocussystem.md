

- UIKit
-  UIFocusSystem 

Class

# UIFocusSystem

Queries and reevaluates the currently focused item.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
class UIFocusSystem
```

## Overview

Use a UIFocusSystem object to obtain the focus-related state for the objects of your app. You can get state information for your app’s views, view controllers, windows, and other objects that adopt the UIFocusEnvironment protocol. The UIFocusSystem object lists the currently focused item, if any, for a window or view hierarchy. You can use it to force the system to update the focus state, and you can register custom sounds to be played during focus changes.

## Topics

### Getting a focus system object

init?(for: any UIFocusEnvironment)

Retrieves a focus system object that contains the state information for the specified object.

Deprecated

class func focusSystem(for: any UIFocusEnvironment) -> UIFocusSystem?

Retrieves the focus system for the specified environment.

### Getting the currently focused item

var focusedItem: (any UIFocusItem)?

The item that’s currently focused.

### Managing focus updates

func requestFocusUpdate(to: any UIFocusEnvironment)

Submits a request to update the focus state of the specified object.

func updateFocusIfNeeded()

Forces the system to act on a pending focus update for the current environment.

### Registering custom sounds

class func register(URL, forSoundIdentifier: UIFocusSoundIdentifier)

Registers the specified sound file with the focus engine.

### Responding to focus-related keys and notifications

class let animationCoordinatorUserInfoKey: String

Updates the animation coordinator.

class let didUpdateNotification: NSNotification.Name

The focus for the UI has been updated.

class let focusUpdateContextUserInfoKey: String

Updates the context key.

class let movementDidFailNotification: NSNotification.Name

The focus failed to move to another item.

## Relationships

### Inherits From

- NSObject

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

class UIFocusUpdateContext

An object that provides information relevant to a specific focus update from one view to another.

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

