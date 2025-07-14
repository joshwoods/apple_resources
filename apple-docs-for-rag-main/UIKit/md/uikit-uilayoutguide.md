

- UIKit
-  UILayoutGuide 

Class

# UILayoutGuide

A rectangular area that can interact with Auto Layout.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class UILayoutGuide
```

## Overview

Use layout guides to replace the placeholder views you may have created to represent inter-view spaces or encapsulation in your user interface. Traditionally, there were a number of Auto Layout techniques that required placeholder views. A placeholder view is an empty view that does not have any visual elements of its own and serves only to define a rectangular region in the view hierarchy. For example, if you wanted to use constraints to define the size or location of an empty space between views, you needed to use a placeholder view to represent that space. If you wanted to center a group of objects, you needed a placeholder view to contain those objects. Similarly, placeholder views could be used to contain and encapsulate part of your user interface. Placeholder views let you break up a large, complex user interface into self-contained, modular chunks. When used properly, they could greatly simplify your Auto Layout constraint logic.

There are a number of costs associated with adding placeholder views to your view hierarchy. First, there is the cost of creating and maintaining the view itself. Second, the placeholder view is a full member of the view hierarchy, which means that it adds overhead to every task the hierarchy performs. Worst of all, the invisible placeholder view can intercept messages that are intended for other views, causing problems that are very difficult to find.

The UILayoutGuide class is designed to perform all the tasks previously performed by placeholder views, but to do it in a safer, more efficient manner. Layout guides do not define a new view. They do not participate in the view hierarchy. Instead, they simply define a rectangular region in their owning view’s coordinate system that can interact with Auto Layout.

### Creating Layout Guides

To create a layout guide, you must perform the following steps:

1.  Instantiate a new layout guide.

2.  Add the layout guide to a view by calling the view’s addLayoutGuide(_:) method.

3.  Define the position and size of the layout guide using Auto Layout.

You can use these guides to define the space between elements in your layout. The following example shows layout guides used to define an equal spacing between a series of views.

- Swift
- Objective-C

```
let space1 = UILayoutGuide()
view.addLayoutGuide(space1)

let space2 = UILayoutGuide()
view.addLayoutGuide(space2)

space1.widthAnchor.constraintEqualToAnchor(space2.widthAnchor).active = true
saveButton.trailingAnchor.constraintEqualToAnchor(space1.leadingAnchor).active = true
cancelButton.leadingAnchor.constraintEqualToAnchor(space1.trailingAnchor).active = true
cancelButton.trailingAnchor.constraintEqualToAnchor(space2.leadingAnchor).active = true
clearButton.leadingAnchor.constraintEqualToAnchor(space2.trailingAnchor).active = true
```

```
UILayoutGuide *space1 = [[UILayoutGuide alloc] init];
[self.view addLayoutGuide:space1];

UILayoutGuide *space2 = [[UILayoutGuide alloc] init];
[self.view addLayoutGuide:space2];

[space1.widthAnchor constraintEqualToAnchor:space2.widthAnchor].active = YES;
[self.saveButton.trailingAnchor constraintEqualToAnchor:space1.leadingAnchor].active = YES;
[self.cancelButton.leadingAnchor constraintEqualToAnchor:space1.trailingAnchor].active = YES;
[self.cancelButton.trailingAnchor constraintEqualToAnchor:space2.leadingAnchor].active = YES;
[self.clearButton.leadingAnchor constraintEqualToAnchor:space2.trailingAnchor].active = YES;
```

A layout guide can also act as an opaque box that contains other views and controls, letting you encapsulate parts of your view and break up your layout into modular chunks.

- Swift
- Objective-C

```
let container = UILayoutGuide()
view.addLayoutGuide(container)

// Set interior constraints
label.lastBaselineAnchor.constraintEqualToAnchor(textField.lastBaselineAnchor).active = true
label.leadingAnchor.constraintEqualToAnchor(container.leadingAnchor).active = true
textField.leadingAnchor.constraintEqualToAnchor(label.trailingAnchor, constant: 8.0).active = true
textField.trailingAnchor.constraintEqualToAnchor(container.trailingAnchor).active = true
textField.topAnchor.constraintEqualToAnchor(container.topAnchor).active = true
textField.bottomAnchor.constraintEqualToAnchor(container.bottomAnchor).active = true

// Set exterior constraints
// The contents of the container can be treated as an opaque box
let margins = view.layoutMarginsGuide

container.leadingAnchor.constraintEqualToAnchor(margins.leadingAnchor).active = true
container.trailingAnchor.constraintEqualToAnchor(margins.trailingAnchor).active = true
container.topAnchor.constraintEqualToAnchor(topLayoutGuide.bottomAnchor, constant: 20.0).active = true
```

```
UILayoutGuide *container = [[UILayoutGuide alloc] init];
[self.view addLayoutGuide:container];

// Layout the contents of the container
[self.label.lastBaselineAnchor constraintEqualToAnchor:self.textField.lastBaselineAnchor].active = YES;
[self.label.leadingAnchor constraintEqualToAnchor:container.leadingAnchor].active = YES;
[self.textField.leadingAnchor constraintEqualToAnchor:self.label.trailingAnchor constant:8.0].active = YES;
[self.textField.trailingAnchor constraintEqualToAnchor:container.trailingAnchor].active = YES;
[self.textField.topAnchor constraintEqualToAnchor:container.topAnchor].active = YES;
[self.textField.bottomAnchor constraintEqualToAnchor:container.bottomAnchor].active = YES;

// Set exterior constraints.
UILayoutGuide *margins = self.view.layoutMarginsGuide;

[container.leadingAnchor constraintEqualToAnchor:margins.leadingAnchor].active = YES;
[container.trailingAnchor constraintEqualToAnchor:margins.trailingAnchor].active = YES;
[container.topAnchor constraintEqualToAnchor:self.topLayoutGuide.bottomAnchor constant:20.0].active = YES;
```

Note

Layout guides provides a lightweight method for encapsulating part of your layout. Note that this technique only affects how Auto Layout interacts with the encapsulated views. It does not change the view hierarchy in any way. However, this is not the only way to create modular user interfaces. Container views and container view controllers provide an even greater degree of encapsulation, letting you separate the layout, the view hierarchy and even the related view controller code. For more information, see Adaptivity and Size Changes in View Controller Programming Guide for iOS.

Additionally, layout constraints do not fully encapsulate their contents. The system still compares the priority of optional constraints inside the layout guide with the priority of optional constraints outside the guide.

## Topics

### Working with layout guides

var identifier: String

A string used to identify the layout guide.

var layoutFrame: CGRect

The layout guide’s frame in its owning view’s coordinate system.

var owningView: UIView?

The view that owns this layout guide.

### Creating constraints using layout anchors

var bottomAnchor: NSLayoutYAxisAnchor

A layout anchor representing the bottom edge of the layout guide’s frame.

var centerXAnchor: NSLayoutXAxisAnchor

A layout anchor representing the horizontal center of the layout guide’s frame.

var centerYAnchor: NSLayoutYAxisAnchor

A layout anchor representing the vertical center of the layout guide’s frame.

var heightAnchor: NSLayoutDimension

A layout anchor representing the height of the layout guide’s frame.

var leadingAnchor: NSLayoutXAxisAnchor

A layout anchor representing the leading edge of the layout guide’s frame.

var leftAnchor: NSLayoutXAxisAnchor

A layout anchor representing the left edge of the layout guide’s frame.

var rightAnchor: NSLayoutXAxisAnchor

A layout anchor representing the right edge of the layout guide’s frame.

var topAnchor: NSLayoutYAxisAnchor

A layout anchor representing the top edge of the layout guide’s frame.

var trailingAnchor: NSLayoutXAxisAnchor

A layout anchor representing the trailing edge of the layout guide’s frame.

var widthAnchor: NSLayoutDimension

A layout anchor representing the width of the layout guide’s frame.

### Debugging the layout guide

func constraintsAffectingLayout(for: NSLayoutConstraint.Axis) -> [NSLayoutConstraint]

The constraints that impact the layout of the guide.

var hasAmbiguousLayout: Bool

A Boolean value indicating whether the constraints impacting the layout guide specify its location ambiguously.

### Handling keyboard layout

var keyboardLayoutGuide: UIKeyboardLayoutGuide

A layout guide that tracks the keyboard’s position in your app’s layout.

class UIKeyboardLayoutGuide

A layout guide that represents the space the keyboard occupies in your app’s layout.

class UITrackingLayoutGuide

A layout guide that automatically activates and deactivates layout constraints depending on its proximity to edges.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIFocusGuide
- UITrackingLayoutGuide

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable
- UIPopoverPresentationControllerSourceItem

## See Also

### Layout guides

class NSLayoutDimension

A factory class for creating size-based layout constraint objects using a fluent API.

