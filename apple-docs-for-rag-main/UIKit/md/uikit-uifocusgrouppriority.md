

- UIKit
-  UIFocusGroupPriority 

Structure

# UIFocusGroupPriority

The importance of an item within a focus group, used by the focus system to determine the group’s primary item.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct UIFocusGroupPriority
```

## Topics

### Constants

static let ignored: UIFocusGroupPriority

The lowest focus group priority, assigned by default.

static let previouslyFocused: UIFocusGroupPriority

The focus group priority of a previously focused item.

static let prioritized: UIFocusGroupPriority

The focus group priority that indicates an item is more important than others.

static let currentlyFocused: UIFocusGroupPriority

The focus group priority of the currently focused item, the highest possible priority.

### Initializing a focus group priority

init(Int)

Creates a focus group priority with the specified value.

init(rawValue: Int)

Creates a focus group priority with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
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

