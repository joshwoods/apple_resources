

- Objective-C Runtime
- NSObject
-  UIAccessibilityAction 

API Collection

# UIAccessibilityAction

A set of methods that accessibility elements can use to support specific actions.

## Overview

The `UIAccessibilityAction` informal protocol provides a way for accessibility elements to support specific actions, such as selecting values in a range or scrolling through information on the screen. For example, to respond to a scrolling gesture, you implement the accessibilityScroll(_:) method and post pageScrolled with the new page status (such as “Page 3 of 9”). Or, to make an element such as a slider or picker view accessible, you first need to characterize it by including the adjustable trait. Then, you must implement the accessibilityIncrement() and accessibilityDecrement() methods. When you do this, assistive technology users can adjust the element using gestures specific to the assistive technology.

## Topics

### Performing an action

func accessibilityActivate() -> Bool

Tells the element to activate itself and report the success or failure of the operation.

func accessibilityIncrement()

Tells the accessibility element to increment the value of its content.

func accessibilityDecrement()

Tells the accessibility element to decrement the value of its content.

func accessibilityScroll(UIAccessibilityScrollDirection) -> Bool

Scrolls screen content in an application-specific way and returns the success or failure of the action.

func accessibilityPerformEscape() -> Bool

Dismisses a modal view and returns the success or failure of the action.

func accessibilityPerformMagicTap() -> Bool

Performs a salient action.

### Accessing custom actions

var accessibilityCustomActions: [UIAccessibilityCustomAction]?

An array of custom actions to display along with the built-in actions.

### Constants

enum UIAccessibilityScrollDirection

The direction of a scrolling action.

## See Also

### Related Documentation

Accessibility Programming Guide for iOS

### Improving Accessibility

UIAccessibility

A set of methods that provides accessibility information about views and controls in an app’s user interface.

UIAccessibilityContainer

Provide a set of methods that view subclasses use to make subcomponents accessible as separate elements.

UIAccessibilityFocus

An informal protocol that provides a way to determine whether an assistive app, such as VoiceOver, has focus on an accessible element.

UIAccessibilityDragging

A pair of properties to allow you to fine-tune how drags and drops are exposed to assistive technologies.

