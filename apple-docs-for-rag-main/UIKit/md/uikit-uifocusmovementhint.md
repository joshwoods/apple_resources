

- UIKit
-  UIFocusMovementHint 

Class

# UIFocusMovementHint

Provides movement hint information for the focused item.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
class UIFocusMovementHint
```

## Topics

### Moving focus

var movementDirection: CGVector

A vector representing how close focus is to moving to another item in the swiped direction.

### Transforming a hint

var interactionTransform: CATransform3D

A 3D transform that contains the combined transformations of perspective, rotation, and translation.

var perspectiveTransform: CATransform3D

A 3D transform that represents a perspective matrix to be applied to match UIKit interaction hinting.

var rotation: CGVector

A vector to apply to a transform to match system interaction hinting.

var translation: CGVector

A vector to apply to a transform to match system interaction hinting.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

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

protocol UIFocusItemContainer

The container responsible for providing geometric context to focus items within a given focus environment.

protocol UIFocusItemScrollableContainer

A type of focus item container that supports automatic scrolling of focusable content.

struct UIFocusGroupPriority

The importance of an item within a focus group, used by the focus system to determine the group’s primary item.

