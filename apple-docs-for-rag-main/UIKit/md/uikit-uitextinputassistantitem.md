

- UIKit
-  UITextInputAssistantItem 

Class

# UITextInputAssistantItem

An object that manages custom bar button items that you add to the shortcuts bar above the keyboard on iPad.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 2.0+

``` source
@MainActor
class UITextInputAssistantItem
```

## Overview

Use a UITextInputAssistantItem object to add app-specific actions to the shortcuts bar on iPad. The center of the shortcuts bar displays typing suggestions for the user. You can install custom bar button items that lead or trail the typing suggestions.

Note

You can add custom items to the shortcuts bar on iPad only. On iPhone, the text input system ignores the contents of the UITextInputAssistantItem object.

You don’t create instances of this class directly. Instead, you get an input assistant from the inputAssistantItem property of the responder object whose keyboard you want to modify. When the keyboard is onscreen, UIKit automatically searches the responder chain for a text-input assistant object. Typically, you assign the text-input assistant to the object that becomes the first responder. However, you can also assign it to a parent responder object to share a set of shortcuts among multiple children.

Organize the bar button items you create for the shortcuts bar into groups. A UIBarButtonItemGroup object manages each group of items, and each group may contain a single item or several items. UIKit displays as many items as possible based on the available space. When there’s not enough space for all of the items, UIKit collapses each group of items down to a single representative item.

The following code configures the items of the shortcuts bar. After creating the bar button items, this code creates a group and assigns that group to the leadingBarButtonGroups property. The resulting items appear before the typing suggestions.

- Swift
- Objective-C

```
// Get a UITextView object of the current view controller.
let item = textView.inputAssistantItem

// Set up the buttons.
let itemOne = UIBarButtonItem(
    title: "One",
    style: .plain,
    target: self,
    action: Selector("handleItemOne:"))
let itemTwo = UIBarButtonItem(
    title: "Two",
    style: .plain,
    target: self,
    action: Selector("handleItemTwo:"))
let itemThree = UIBarButtonItem(
    title: "Three",
    style: .plain,
    target: self,
    action: Selector("handleItemThree:"))

// Use a nil action to display the individual items.
let itemChoose = UIBarButtonItem(
    title: "Choose",
    style: .plain,
    target: nil,
    action: nil)

// Create the item group.
let group = UIBarButtonItemGroup(
    barButtonItems: [itemOne, itemTwo, itemThree],
    representativeItem: itemChoose)

// Display the items before the typing suggestions.
item.leadingBarButtonGroups = [group]
```

```
// Get a UITextView object of the current view controller.
UITextInputAssistantItem* item = [self.textView inputAssistantItem];

// Set up the buttons.
UIBarButtonItem* itemOne = [[UIBarButtonItem alloc] initWithTitle:@"One"
         style:UIBarButtonItemStylePlain target:self action:@selector(handleItemOne:)];
UIBarButtonItem* itemTwo = [[UIBarButtonItem alloc] initWithTitle:@"Two"
         style:UIBarButtonItemStylePlain target:self action:@selector(handleItemTwo:)];
UIBarButtonItem* itemThree = [[UIBarButtonItem alloc] initWithTitle:@"Three"
         style:UIBarButtonItemStylePlain target:self action:@selector(handleItemThree:)];

// Use a nil action to display the individual items.
UIBarButtonItem* itemChoose = [[UIBarButtonItem alloc] initWithTitle:@"Choose"
         style:UIBarButtonItemStylePlain target:nil action:nil];

// Create the item group.
UIBarButtonItemGroup* group = [[UIBarButtonItemGroup alloc]
       initWithBarButtonItems:@[itemOne, itemTwo, itemThree] representativeItem:itemChoose];

// Display the items before the typing suggestions.
item.leadingBarButtonGroups = @[group];
```

To hide shortcuts altogether, set the leadingBarButtonGroups and trailingBarButtonGroups properties to empty arrays. Doing so hides only the shortcuts and doesn’t hide the typing suggestions. For information on managing the typing suggestions, see autocorrectionType.

## Topics

### Configuring the shortcuts bar

var leadingBarButtonGroups: [UIBarButtonItemGroup]

The array of button item groups to display before the typing suggestions.

var trailingBarButtonGroups: [UIBarButtonItemGroup]

The array of button item groups to display after the typing suggestions.

var allowsHidingShortcuts: Bool

A Boolean value that indicates whether the user can hide the shortcuts bar.

### Instance Properties

var keyboardAction: UIBarButtonItem?

A button that appears next to the text preview in the keyboard in visionOS.

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

### Text input

protocol UITextInput

A set of methods for interacting with the text input system and enabling features in documents.

protocol UITextInputDelegate

An intermediary between a document and the text input system.

protocol UIKeyInput

A set of methods a responder uses to implement simple text entry.

protocol UITextInputTraits

A set of methods that defines features for keyboard input to a text object.

class UITextInputContext

An object that reports the type of input your app receives.

class UITextInputMode

The current text input mode.

class UIDictationPhrase

An object that represents the textual interpretation of a spoken phrase that the user dictates.

