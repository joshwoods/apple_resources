

- Objective-C Runtime
- NSObject
-  UIAccessibilityDragging 

API Collection

# UIAccessibilityDragging

A pair of properties to allow you to fine-tune how drags and drops are exposed to assistive technologies.

## Overview

By default, if an accessible view or its subtree has drag and/or drop interactions, they will be automatically exposed by assistive technologies. However, if there is more than one such interaction, each drag or drop should have a name to disambiguate it and give a good user experience. Also, there may be situations in which you want to expose drags or drops from an element, and those interactions are installed on views that are not part of that element’s view hierarchy subtree.

This is trivially the case when the element is not a view at all, but an instance of `UIAccessibilityElement`.

Another example is when a container view maintains interactions that are logically associated with subviews.

For instance, `UITableView` has associated drag interactions that allow for dragging its rows; to make the rows draggable by assistive technologies, `UITableViewCell` has drag descriptors that describe where in the table view to start a drag to activate dragging of the cell.

Note

This implementation detail is noted here for expository purposes only and may change at any time without warning.

Properties defined here allow you to fine-tune how drags and drops are exposed to assistive technologies. Both of their getter methods can be overridden to provide information on-demand.

For each location descriptor, the associated view should be the `UIView` with the appropriate `UIInteraction` object for that drag or drop.

## Topics

### Fine-Tuning Drag and Drop

var accessibilityDragSourceDescriptors: [UIAccessibilityLocationDescriptor]?

An array of location descriptor objects that you use to define what drags are possible from this element.

var accessibilityDropPointDescriptors: [UIAccessibilityLocationDescriptor]?

An array of location descriptor objects that you use to define where drops are possible on this element.

## See Also

### Related Documentation

Accessibility Programming Guide for iOS

### Improving Accessibility

UIAccessibility

A set of methods that provides accessibility information about views and controls in an app’s user interface.

UIAccessibilityContainer

Provide a set of methods that view subclasses use to make subcomponents accessible as separate elements.

UIAccessibilityAction

A set of methods that accessibility elements can use to support specific actions.

UIAccessibilityFocus

An informal protocol that provides a way to determine whether an assistive app, such as VoiceOver, has focus on an accessible element.

