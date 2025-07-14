

- UIKit
-  UIFocusItemScrollableContainer 

Protocol

# UIFocusItemScrollableContainer

A type of focus item container that supports automatic scrolling of focusable content.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
@MainActor
protocol UIFocusItemScrollableContainer : UIFocusItemContainer
```

## Overview

The focus engine scrolls the container to keep items onscreen as they become focused. This is done by repeatedly setting contentOffset.

## Topics

### Retrieving the content size

var contentOffset: CGPoint

The current content offset for the scrollable container.

**Required**

var contentSize: CGSize

The total size of the content contained by this container.

**Required**

var visibleSize: CGSize

The visible size of the scrollable container.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UIFocusItemContainer

### Conforming Types

- UICollectionView
- UIScrollView
- UITableView
- UITextView

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

class UIFocusUpdateContext

An object that provides information relevant to a specific focus update from one view to another.

protocol UIFocusItem

An object that can become focused.

class UIFocusMovementHint

Provides movement hint information for the focused item.

protocol UIFocusItemContainer

The container responsible for providing geometric context to focus items within a given focus environment.

struct UIFocusGroupPriority

The importance of an item within a focus group, used by the focus system to determine the group’s primary item.

