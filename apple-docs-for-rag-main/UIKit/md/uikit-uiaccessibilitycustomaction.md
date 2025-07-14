

- UIKit
-  UIAccessibilityCustomAction 

Class

# UIAccessibilityCustomAction

A custom action to perform on an accessible object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIAccessibilityCustomAction
```

## Overview

Apps that support custom actions can create instances of this class, specifying the user-readable name of the action and the object and selector to use when performing the action. Assistive apps display custom actions in response to specific user cues. For example, VoiceOver lets users access actions quickly using the Actions rotor.

After creating an instance of this class, add it to the accessibilityCustomActions property of an appropriate accessible object.

## Topics

### Creating a custom action

init(name: String, actionHandler: UIAccessibilityCustomAction.Handler)

Creates a custom action object with the specified name and action handler.

init(name: String, target: Any?, selector: Selector)

Creates a custom action object with the specified name, target, and selector.

init(name: String, image: UIImage?, actionHandler: UIAccessibilityCustomAction.Handler)

Creates a custom action object with the specified name, image, and action handler.

init(name: String, image: UIImage?, target: Any?, selector: Selector)

Creates a custom action object with the specified name, image, target, and selector.

init(attributedName: NSAttributedString, actionHandler: UIAccessibilityCustomAction.Handler)

Creates a custom action object with the specified attributed name and action handler.

init(attributedName: NSAttributedString, target: Any?, selector: Selector)

Creates a custom action object with the specified attributed name, target, and selector.

init(attributedName: NSAttributedString, image: UIImage?, actionHandler: UIAccessibilityCustomAction.Handler)

Creates a custom action object with the specified attributed name, image, and action handler.

init(attributedName: NSAttributedString, image: UIImage?, target: Any?, selector: Selector)

Creates a custom action object with the specified attributed name, image, target, and selector.

### Accessing the action parameters

var name: String

The localized name of the action.

var attributedName: NSAttributedString

The localized name of the action as an attributed string.

var image: UIImage?

An image that represents the action in assistive apps.

var actionHandler: UIAccessibilityCustomAction.Handler?

A handler to perform for the action.

var target: AnyObject?

The object that performs the action.

var selector: Selector

The method that performs the action.

typealias Handler

A closure type that defines a handler to perform for an action.

### Type Properties

class let editCategory: String

### Instance Properties

var category: String?

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

### Actions

UIAccessibilityAction

A set of methods that accessibility elements can use to support specific actions.

typealias Handler

A closure type that defines a handler to perform for an action.

Delivering an exceptional accessibility experience

Make improvements to your app’s interaction model to support assistive technologies such as VoiceOver.

